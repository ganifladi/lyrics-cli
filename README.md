# lyrics-cli
<p>This repo includes a version of <a href="https://github.com/nick-parry/songLyrics">songLyrics</a> with <b>DuckDuckGo</b> search and fetches song information from mpv or mpd. The other script is a enhanced version of <a href="https://github.com/xanpdx/lyric-scripts">songLyricsFormatted</a>, which shows the fetched lyrics formatted in three lines. The next three lines will either roll on automatically via time or manually via keypress. You can also easily register when rolls the lyrics the first time, and the next time it will scoll automatically.</p>
<h2>How to install</h2>
<ol>
<li>Download the two scripts and place them in a directory e.g. "~/.scripts"</li>
<li>Modify the save paths at the beginnig of the two files, or leave the default</li>
<li>Make them executable, with `chmod +x _pathToFile_`.</li>
</ol>
<h2>How to use</h2>
<ol>
<li>Start mpv or mpd and the song you want to listen to</li>
<li>Run the script with ~/.scripts/lyricsFormat _parameters_</li>
<li>Enjoy the lyrics inside your terminal</li>
</ol>
<h2>Parameters</h2>
<li>**-s**: Save the lyrics to the lyrics folder. If it already exists, don't overwrite.</li>
<li>**-S**: As above, but will overwrite existing files.</li>
<li>**-r**: It will register the time when you press enter to scroll the lyrics, and save it to a file in the timing directory. This file will be read to know when to auto scroll. Doesn't overwrites existing files. If the file already exists, it will only show the lyrics, without recording.</li>
<li>**-R**: As above, but will overwrite existing files.</li>
<li>**mpd** or **mpv**: the music server/deamon you want to use.</li>
</ol>
<h3>Default values and behavior</h3>
<p>Without parameters, the program will not save, will not record and will fetch the music data from mpd (you can change the default value at the beginning of the script). It will automatically scrolls the lyrics if the timing has been previously recorded. It will take the lyrics from the saved file (if exists), or search it in the internet.</p>
<p>If you just want the lyrics to autoroll after a prefixed and constant time, change the commented lines in "lyricsFormat"s source.</p>
<p>Have fun.</p>
