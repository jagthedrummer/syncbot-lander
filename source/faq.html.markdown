---
title: FAQ
layout: markdown
---

# Can I use symlinks instead of putting projects directly in `~Syncbot`?

Well... kinda?

If Syncbot is running when you create a symlink it should notice the new project
and the project should be uploaded.

**However** the process that watches for changes in the
`~/Syncbot` directory won't be able to "see" any changes in the project. That means
that **if you save a change to the project Syncbot won't automatically upload it for you.**
If you quit and then restart Syncbot it should see the changes on the initial scan
and then upload the new version at that time. You'll need to restart Syncbot each time
that you've made a change you want to upload.

**For best results I recommend putting projects directly in the `~/Syncbot` folder,
or in one of its sub-folders.**

In the future there _might_ be a configuration option to let you tell Syncbot to
watch other folders.

