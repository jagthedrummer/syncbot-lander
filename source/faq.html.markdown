---
title: FAQ
layout: markdown
---

# FAQ

## Can I use symlinks instead of putting projects directly in `~Syncbot`?

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

## Will Syncbot mess up my sessions?

_I certainly hope not!_

But, with that being said, you should be aware that that **Syncbot is alpha level software**. For
now I'd recommend being cautious, and if you have sessions that you really care about, please
keep a copy of them outside of Syncbot.

In most cases Syncbot won't do things that would mess up a session.

But some actions are riskier than others. In specific, any time you download a project (or an
older version), there is a chance for something to go sideways since we're directly messing
with files inside the session.

Be sure to close Logic or Ableton before downloading new versions of a project.

Non-risky activities:

* If you're using Syncbot on your own, to back up your sessions, and you're not
  going back to older versions then there is very little risk that Syncbot could
  mess up your sessions.


