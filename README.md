---


---

<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.<br>
**</p>
</blockquote>
<h2 id="news-feed-app">News Feed App</h2>
<p>The App is available here: <a href="https://newsnote.netlify.app/">NoteNews</a></p>
<p>This is a full stack web app using MERN technology.<br>
Key features are:</p>
<ul>
<li><strong>Landing Page</strong> with Login/Register feature.<br>
<img src="https://i.imgur.com/uwBvWNw.gif" alt="enter image description here"><br>
<img src="https://i.imgur.com/w27S1wM.png" alt="enter image description here"><br>
<img src="https://i.imgur.com/p3rn7l9.png" alt="enter image description here"></li>
<li>After logging in, the <strong>homepage</strong> will pull the latest news happening in the world from GNEWS API.<br>
<img src="https://i.imgur.com/X10Lmky.png" alt="enter image description here"></li>
<li><strong>Notes Hub</strong> section will display notes written by different users<br>
<img src="https://i.imgur.com/7uzOp9r.png" alt="enter image description here"></li>
<li><strong>Add notes page</strong> will allow user to add their notes to the Notes Hub.<br>
<img src="https://i.imgur.com/SP051Mc.png" alt="enter image description here"></li>
<li><strong>My Notes</strong> page will allow you to see your own posted notes and make modification or deletion.<br>
<img src="https://i.imgur.com/WUV4QF8.png" alt="enter image description here"></li>
</ul>
<h2 id="key-features-that-fulfill-the-requirements">Key Features that fulfill the requirements:</h2>
<p>Since there are requirements for this project, let me present which part of my app meets those requirements, so you don’t have to spend time looking.</p>
<ul>
<li class="task-list-item">
<p><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled=""> Languages: I used TypeScript as the language choice and backend running on Express server on Node.js runtime.</p>
</li>
<li class="task-list-item">
<p><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled=""> UI Design:<br>
Hierarchy implementation:</p>
</li>
<li>
<p>Place important actions at the top or side of the screen, like navbar/sidebar.</p>
</li>
<li>
<p>Place related items of a similar hierarchy next to each other.</p>
</li>
</ul>
<p>Grouping:</p>
<ul>
<li>Items can be grouped under headings that communicate what the groupings are. These groups organize content spatially.</li>
</ul>
<p>Contrast ratios:</p>
<ul>
<li>Use higher contrast makes the imagery easier to see. Icons follow the color contrast ratio recommendations and are legible against their backgrounds.</li>
</ul>
<p>Indicating elements by action:</p>
<ul>
<li>Instead of showing the icon only, have the text next to it describes what an element does without relying on visual acuity.</li>
</ul>
<p>Use proper “alt” for image:</p>
<ul>
<li>If the image is purely decorative, can leave the alt empty (alt=""), for news image, it might or might not be decorative, so if the parameter from the API has something like <code>alt_text</code>, we can use that in our <code>&lt;img&gt;</code> tag.</li>
</ul>
<br>
<br>
<ul>
<li class="task-list-item">
<p><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled=""> Architecture Pattern:</p>
</li>
<li>
<p>App has <strong>frontend</strong> and <strong>backend</strong> two main parts.</p>
</li>
<li>
<p>Frontend has <strong>pages</strong> including several pages to display content for the website. It also has <strong>components</strong> folder containing <strong>Sidebar</strong>, <strong>Layout</strong> and <strong>Spinner</strong> (for loading animation) used in different pages as <strong>reusable components</strong>.</p>
</li>
<li>
<p>Backend has two main folders:<br>
<strong>models</strong>: containing schemas for creating post and creating user.<br>
<strong>routes</strong>: containing <strong>newsRoute</strong> and <strong>userRoute</strong>. newsRoute is responsible for the <strong>CRUD</strong> operations of creating new notes to the notes hub page, edit and delete user’s own notes, and get all notes posted by all users.<br>
userRoute is responsible for registering and login functionality.</p>
</li>
</ul>
<p>Please refer to the diagram below for the pattern. (For higher resolution please visit: <a href="https://drive.google.com/file/d/1W5talZAwembN65RcU1DDmTFSBpxgUSZN/view?usp=sharing">link</a>)</p>
<p><img src="https://i.imgur.com/sM0IGkZ.png" alt="image"></p>
<br>
<ul>
<li class="task-list-item"><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled=""> 3rd Party API<br>
This app uses the news feed API from <a href="http://GNews.io">GNews.io</a> (<a href="https://gnews.io/docs/v4#introduction">https://gnews.io/docs/v4#introduction</a>)</li>
</ul>
<p>I’m using the free tier so it will retrieve 10 news per request. The country has been set to US. Here are the results.<br>
<img src="https://i.imgur.com/X10Lmky.png" alt="image"></p>
<ul>
<li class="task-list-item">
<p><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled=""> At least 5 mererial-UI icons.<br>
<img src="https://i.imgur.com/JsaQjZT.png" alt="enter image description here"><br>
<img src="https://i.imgur.com/efsuHRE.png" alt="enter image description here"><br>
<img src="https://i.imgur.com/3YNxc5d.png" alt="enter image description here"><br>
<img src="https://i.imgur.com/o5iabQP.png" alt="enter image description here"><br>
<img src="https://i.imgur.com/QMtCwW0.png" alt="enter image description here"><br>
<br><br>
<br><br>
<br></p>
</li>
<li class="task-list-item">
<p><input type="checkbox" class="task-list-item-checkbox" checked="true" disabled=""> Example of reusable component:<br>
As you can see from the previous webpage picture. The sidebar and top header are universal across every page. Also, the edit notes page and add notes page share the same structure, as well as login and register UI, they share the same UI design.</p>
</li>
</ul>

