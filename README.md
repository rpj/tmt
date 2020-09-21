# TileMapTool

A single-file, [no-dependency](http://vanilla-js.com/), offline-capable tool for exploring, annotating & exporting tilemaps.

## Running

### Locally

[Download `index.html`](https://raw.githubusercontent.com/rpj/tmt/main/index.html) and open it. That's it.

### Online

At [GitHub Pages](https://rpj.github.io/tmt/), [itch.io](https://rpjsf.itch.io/tmt/) or [computerpho.be](https://tmt.computerpho.be/).

<!-- The "Usage" section must be pure HTML to allow pulling it into the tool directly -->
## Usage

<p>Explore the default map or load another: built-in maps will automatically set the correct parameters. If loading from disk, proceed to set the appropriate "tile w/h" (width/height) and "spacing" parameters via the controls; all control changes are reflected on the tilemap live. The control value label is double-clickable to allow arbitrary input (caveat emptor!).</p>

<p>Click on any tile to select & have it displayed in the larger "selected" view, which shows the tile's X & Y coordinates (in <i>tile coordinate space</i>) as well as the top-left and bottom-right coordinates of the tile in the <i>source image coordinate space</i>. The selection can also be moved with the arrow keys.</p>

<p>Right-click any tile to annotate it with a group & name. Once annotation mode has been entered - implicitly by creating the first annotation group - tilemap loading & parameter controls will be locked (though viewport controls will remain available).</p>

<p>In annotation mode, additional controls will become availble beneath the selected view:</p>

<ul>
<li><b>"Save JSON"</b>: Creates & downloads a JSON file describing the annotated tiles and their positions on the currently-loaded tilemap in both tile-coordinate & pixel-coordinate spaces.</li>
<li><b>"Export New"</b>: Creates a new PNG image containing <i>only</i> the annotated tiles as well as a JSON file with the appropriate annotation metadata in the same shape as "Save JSON" above. This option will initiate multiple downloads, which your browser may require you explicitly allow.</li>
<li><b>"Discard"</b>: Immediately discards all current annotations and returns to the default mode, re-enabling tilemap loading & parameter controls.</li>
</ul>

## Screenshots

![Screenshot 1](https://tmt.computerpho.be/ss1.png)
![Screenshot 2](https://tmt.computerpho.be/ss2.png)
![Screenshot 3](https://tmt.computerpho.be/ss3.png)