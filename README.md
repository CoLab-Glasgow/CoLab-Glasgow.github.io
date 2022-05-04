# CoLab Webpage

This README contains instructions on how to add more info to the CoLab webpage. Most styling has already been set, so just focus on adding the info! I am using the [milligram](https://milligram.io/) (lightweight) CSS framework for styling, take a look to see a full list of what you can do!

## Adding team member

To add a new team member to the `Team` section, paste in _one_ of the following to `index.html` above the line marked `<!-- TO ADD NEW TEAM MEMBERS, PASTE ABOVE THIS LINE -->` and fill in the necessary details.

Option 1 (Image on the _left_): 
```html
<!-- Photo on the left -->
<div class="row tinted-bg">
    <div class="column">
        <div class="container">
            <!-- Name header -->
            <div class="row no-padding">
                <div class="column"><h4>[NAME]</h4></div>
            </div>

            <div class="row no-padding">
                <!-- IMG of team member -->
                <div class="column column-25">
                    <img src="images/[LINK TO IMG]" alt="Photo of [NAME]">
                </div>
                <!-- About team member -->
                <div class="column column-75">
                    <div class="container">
                        <div class="row no-padding">
                            <div class="column">
                                <p>
                                    [PERSONAL DETAILS]
                                </p>
                            </div>
                        </div>
                        <!-- Links and socials -->
                        [SOCIALS]
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
```

__OR__

Option 2 (Image on the _right_): 
```html
<!-- Photo on the right -->
<div class="row tinted-border">
    <div class="column">
        <div class="container">
            <!-- Name header -->
            <div class="row no-padding">
                <div class="column"><h4>[NAME]</h4></div>
            </div>

            <div class="row no-padding">
                <!-- About team member -->
                <div class="column column-75">
                    <div class="container">
                        <div class="row no-padding">
                            <div class="column">
                                <p>
                                    [PERSONAL DETAILS]
                                </p>
                            </div>
                        </div>
                        [SOCIALS]
                    </div>
                </div>
                <!-- IMG of team member -->
                <div class="column column-25">
                    <img src="images/[LINK TO IMG].jpg" alt="Photo of [NAME]">
                </div>
            </div>
        </div>
    </div>
</div>
```

A sample for `[SOCIALS]` is:
```html
<div class="row">
    <div class="column center">
        <a class="button" href="[LINK TO DBLP]">dblp</a>
    </div>
    <div class="column center">
        <a class="button button-outline center-tag" href="mailto:[EMAIL]">email</a>
    </div>
    <div class="column center">
        <a class="button" href="[LINK TO WEBPAGE]">webpage</a>
    </div>
</div>
```
Feel free to change these default socials per team member. You can add more than 3 if you want too - they will resize and reposition automagically, just try stick to the same CSS pattern.


## Adding papers

To add a new paper to the `Papers` section, paste the following to `index.html` above the line marked `<!-- TO ADD NEW PAPERS, PASTE ABOVE THIS LINE -->` and fill in the necessary details.

```html
<tr>
    <td>[TITLE]</td>
    <td>[VENUE] [YEAR]</td>
    <td>[AUTHORS]</td>
    <td>
        <a href="[LINK TO PUBLICATION]" title="Publication"><i class="fa fa-2x fa-file-pdf-o"></i></a>
        <a href="[LINK TO DBLP BIBTEX]" title="BibTex"><i class="fa fa-2x fa-file-code-o"></i></a>
    </td>
</tr>
```