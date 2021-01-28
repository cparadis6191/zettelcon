# zettelcon

***

## Work in Progress

***

> An additional helper tool to Zettlr to automatically add backlinks to your note files.
> Edits files in-place, so be careful and try on a copy of your files first.
> 
> Also check out [zettelwarmer](https://github.com/whateverforever/zettelwarmer) for finding
> new interconnections between your notes.

## Assumptions

- Note IDs are unique, also relative to the names of the notes
- The backlink section is the last thing of a page
- Two spaces are used for list indentation

## Issues

- If something is quoted in a list, the list is copied over to the backlink section messing up the alignment and formatting
  - Maybe this can be fixed by not going by paragraphs but newlines instead
  - [ ] Clean quotes lines from any markdown symbols before the line begins
- [x] Display first H1 tag in backlink list, if available
  - Needed if the file names are only IDs and don't give any information of the title
- [x] Last letter of Agency, Kanban, Habits is cut off
  - These are all files with no contents besides the heading
- [x] Path in backlinks needs to be relative to markdown file
- [x] Bureaucracy is fucked up
- [x] Not idempotent

## Improvements

- [ ] Only cite a few words before and after the citation
- [ ] Add horizontal break before backlinks
- [x] Put backlinks in > quotation

---

## Next Sprint

- [ ] Output additional info such as islands, sinks, sources, etc.