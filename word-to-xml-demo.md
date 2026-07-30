# Explaining rich text vs. plain text

While we often try to explain the difference between rich and plain text, sometimes it easier to show others what we mean. To users who are only starting to become comfortable with what is hidden on their computer, they may see a Word document or an Excel spreadsheet and think it looks pretty plain if they haven't added much formatting. The steps below help demonstrate how a Word doc is actually a series of folders and XML files. As you explore, you'll see that the text of your word document is in one XML file and wrapped with markup that, combined with the additional files, make it intelligible to Microsoft Word software.

1. Find a word document (in .docx format) and record the file name and its directory (folder).
2. Open terminal
3. Navigate to directory that contains .docx file you want to unzip (open as xml). My file is on my desktop, so I want to navigate to `username desktop %`. Use the change directory command `cd` to change to the proper directory. For example:

```
cd path/to/your/file
```

4. Once you are in the folder with the file you want to explore, use the `unzip` command followed by your file name and then `-d` flag to specify the directory and then `folder-name` to name the directory to put the files. Copy the code snippet below and execute in your terminal (be sure to change `file.docx` and `folder-name` to names relevant to your material):

```
unzip file.docx -d folder-name
```

5. You should now have a new folder with the unzipped files. Open `document.xml` in the `word` folder and you can see all the code wrapped around the text in your word file.