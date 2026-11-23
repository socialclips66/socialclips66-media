# Inbox (cloud deliveries)

Content sessions running in the cloud deliver finished posts here instead of the Mac's "Ready to Post" folder:

- `inbox/videos/<Post Name>/video.mp4` + `post.txt`
- `inbox/carousels/<Post Name>/01.jpg, 02.jpg, …` + `post.txt`
- `inbox/photos/<Post Name>/<files>` + `post.txt`
- Fix for an already scheduled post: `inbox/<type>/<Post Name> (FIX)/` with a post.txt saying what changed.

The scheduling chat reviews each one (QA, facts, hook, series rules), schedules it in Buffer (videos) or Metricool (carousels/photos), then `git mv`s it to `videos|carousels|photos/YYYY-MM-DD-slug/`.
