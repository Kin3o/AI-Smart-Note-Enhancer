<h1>Smart Note Enhancer with Claude API key</h1>

<h2>Description</h2>
In this project I simply prompted codex to create a Smart Note Enhancer to make jumbled, unorganized and difficult to digest notes into a more comprehensive example of notes that I could study and that were more easily digestable. I did not build the program, I am just showing off the powers and capabilities of LLMs and how I use them everyday to improve my effeciency and productivity. I have also created a MP3 audio player that is connected to my "Study Notes" folder in the Obsidian Notes app. The MP3 audio player converts my notes into a comprehensible dialogue that is easy to understand and listen to. I configured the MP3 audio player application to my automatically upload notes that have been untouched for 16 hours into my Icloud. I particulary use this while taking showers or cleaning.
<br />

<h2>Background</h2>
When I type notes for studying for college or certification exams they are typically scrambled, unorganized and not very comprehensible. I used codex(ChatGPT) to build a community plug in for my note taking app Obsidian. This community plugin drastically helps me comprehend notes that I take by making mind maps, flashcards, structured proccesses, definitions, concepts explained simple and organized tables. 
<br />

<h2>Programs and Utilities Used</h2>

- <b>Obsidian</b> 
- <b>Codex</b>

<h2>Before Smart Note Enhancer</h2>
<img src="https://i.imgur.com/WqQ4tf5.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<h2>After Smart Note Enhancer</h2>
<img src="https://i.imgur.com/YPuIFA9.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<h2>After Smart Note Enhancer</h2>
<img src="https://i.imgur.com/G9zbA05.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<h2>After Smart Note Enhancer</h2>
<img src="https://i.imgur.com/24mRKZ8.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<h2>What I did to create this smart note enhancer </h2>
<h3>Download Codex and Obsidia</h3>

Input a command like such

```bash
Build a fully functional Obsidian community plugin called “Smart Note Enhancer.”

The plugin should enhance Markdown notes into structured study notes using the Anthropic Claude API. Use TypeScript, the Obsidian API, and esbuild. The final plugin should be installable by dropping the plugin folder into `.obsidian/plugins/` and enabling it in Obsidian.

Core requirements:

1. Claude API Integration
- Use an Anthropic Claude API key entered by the user in plugin settings.
- Use Claude Sonnet 4.6 with medium thinking capability.
- Add a “Test API Key” button in settings to verify that the key and model work before enhancing notes.
- If the API call fails, log the error and leave the note unchanged.

2. Auto Enhancement
- Track notes created after the plugin is installed.
- Store each note’s creation timestamp in frontmatter.
- Exactly 16 hours after a note is created, enhance that note automatically.
- Do not retroactively enhance old notes unless the user manually triggers enhancement.

3. Folder Safety
- The plugin must never move notes.
- If a note is inside any folder, automatic enhancement should skip it.
- Let users define protected folders in settings.
- Notes in protected folders must never be changed by automation.

4. Manual Enhancement
- Add a ribbon menu button for enhancing the current note.
- When clicked, show a dropdown of enhancement styles before running.
- Add a settings button called “Enhance Current Note” that also lets the user choose a style.

5. Enhancement Styles
Include these styles:
- Cornell Notes
- Mind Map
- Lecture Notes
- Exam Review
- Cybersecurity Lab Notes
- Rough Outline
- Split Page
- MP3 Enhancer

The MP3 Enhancer style should rewrite notes as a narrated lesson optimized for listening, text-to-speech, or audiobook-style review.

6. Generated Note Content
Claude should generate:
- A clear title
- Study snapshot
- Big idea section
- Structured notes
- Mermaid diagrams
- Key terms table
- Flashcards in table format
- Image search callouts
- Context-based Obsidian hashtags at the bottom
- A preserved “Original Note” callout at the bottom

7. Flashcards
- Generate flashcards from the note content.
- Format them as a readable table.
- Make them clickable/flippable in Obsidian using plugin CSS.

8. Progress Widget
- Add a persistent top-right progress widget visible outside settings.
- Show active note name, current stage, progress bar, and percentage.
- Use stage-based progress such as:
  0% Preparing note
  5% Analyzing note structure
  15% Extracting concepts
  30% Building enhancement prompt
  45% Sending to Claude
  60% Generating enhanced content
  75% Processing response
  90% Formatting output
  100% Complete
- The progress bar should update smoothly and not appear frozen.

9. Unenhance Feature
- Add a button to restore an enhanced note back to its preserved original content.
- Create a backup before modifying or restoring notes.

10. Packaging
Include:
- `manifest.json`
- `package.json`
- `tsconfig.json`
- `esbuild.config.mjs`
- `src/main.ts`
- `styles.css`
- `README.md`

Build the complete plugin and verify that it compiles successfully.
```

Aqquire an API from your LLM vender (I used Claude Opus 4.8)<br/>
<img src="https://i.imgur.com/Ya3UtQh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
</p>
