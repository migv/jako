# jako
Webpage for fun

- `index.html` is the main page: links to the current message and the list of older ones
- `message.html` has the current message and is the one to be modified
- `messages/YYYY-MM-DD.html` are the older messages, one page each
- `style.css` is shared by all the pages
- `allmessages.html` is the old archive (messages as HTML comments), not yet migrated

To post a new message: copy `message.html` to `messages/<its-date>.html` (fix the back link to
`../index.html` and the `style.css` path to `../style.css`), add a line for it at the top of
*Older messages* in `index.html`, then write the new message in `message.html` and update its
link and date in `index.html`. Commit as `Message of the day YYYY-MM-DD`.
