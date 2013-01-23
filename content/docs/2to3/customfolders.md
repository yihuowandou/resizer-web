# Migrating CustomFolders.cs

If you have modified CustomFolders.cs, you will need migrate your URL rewriting to use the RewriteDefaults, Rewrite, and PostRewrite events found in ImageResizer.Configuration.Config.Current.Pipeline.

You should register these event handlers in Application_Start (Global.asax).

Alternatively, you could create a Plugin (suggested for easy reuse).