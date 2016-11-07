[INFO] Error stacktraces are turned on.
[INFO] Scanning for projects...
[INFO] 
[INFO] Using the MultiThreadedBuilder implementation with a thread count of 4
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] Building parent 1-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO] 
[INFO] --- maven-site-plugin:3.6:run (default-cli) @ parent ---
[WARNING] Input file encoding has not been set, using platform encoding UTF-8, i.e. build is platform dependent!
[INFO] Logging to Logger[org.mortbay.log]@1522463235 via org.mortbay.log.Slf4jLog
[WARNING] Report plugin org.apache.maven.plugins:maven-project-info-reports-plugin has an empty version.
[WARNING] 
[WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
[WARNING] 
[WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
[INFO] configuring report plugin org.apache.maven.plugins:maven-project-info-reports-plugin:2.9
[WARNING] Report plugin org.apache.maven.plugins:maven-project-info-reports-plugin has an empty version.
[WARNING] 
[WARNING] It is highly recommended to fix these problems because they threaten the stability of your build.
[WARNING] 
[WARNING] For this reason, future Maven versions might no longer support building such malformed projects.
[INFO] configuring report plugin org.apache.maven.plugins:maven-project-info-reports-plugin:2.9
[WARNING] No project URL defined - decoration links will not be relativized!
[INFO] Rendering site with org.apache.maven.skins:maven-fluido-skin:jar:1.6 skin.
[INFO] ------------------------------------------------------------------------
[INFO] BUILD FAILURE
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 1.642 s (Wall Clock)
[INFO] Finished at: 2016-11-07T14:38:12-05:00
[INFO] Final Memory: 18M/239M
[INFO] ------------------------------------------------------------------------
[ERROR] Failed to execute goal org.apache.maven.plugins:maven-site-plugin:3.6:run (default-cli) on project parent: Unable to set up webapp: RendererException while preparing context for skin: Cannot use skin: has 1.7.1 Doxia Sitetools prerequisite, but current is 1.7 -> [Help 1]
org.apache.maven.lifecycle.LifecycleExecutionException: Failed to execute goal org.apache.maven.plugins:maven-site-plugin:3.6:run (default-cli) on project parent: Unable to set up webapp
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:214)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:155)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:147)
    at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject (LifecycleModuleBuilder.java:116)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:185)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:181)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.Executors$RunnableAdapter.call (Executors.java:511)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.ThreadPoolExecutor.runWorker (ThreadPoolExecutor.java:1142)
    at java.util.concurrent.ThreadPoolExecutor$Worker.run (ThreadPoolExecutor.java:617)
    at java.lang.Thread.run (Thread.java:745)
Caused by: org.apache.maven.plugin.MojoExecutionException: Unable to set up webapp
    at org.apache.maven.plugins.site.run.SiteRunMojo.createWebApplication (SiteRunMojo.java:222)
    at org.apache.maven.plugins.site.run.SiteRunMojo.execute (SiteRunMojo.java:87)
    at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo (DefaultBuildPluginManager.java:134)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:209)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:155)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:147)
    at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject (LifecycleModuleBuilder.java:116)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:185)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:181)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.Executors$RunnableAdapter.call (Executors.java:511)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.ThreadPoolExecutor.runWorker (ThreadPoolExecutor.java:1142)
    at java.util.concurrent.ThreadPoolExecutor$Worker.run (ThreadPoolExecutor.java:617)
    at java.lang.Thread.run (Thread.java:745)
Caused by: org.apache.maven.plugin.MojoExecutionException: RendererException while preparing context for skin: Cannot use skin: has 1.7.1 Doxia Sitetools prerequisite, but current is 1.7
    at org.apache.maven.plugins.site.render.AbstractSiteRenderingMojo.createSiteRenderingContext (AbstractSiteRenderingMojo.java:336)
    at org.apache.maven.plugins.site.run.SiteRunMojo.createWebApplication (SiteRunMojo.java:179)
    at org.apache.maven.plugins.site.run.SiteRunMojo.execute (SiteRunMojo.java:87)
    at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo (DefaultBuildPluginManager.java:134)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:209)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:155)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:147)
    at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject (LifecycleModuleBuilder.java:116)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:185)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:181)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.Executors$RunnableAdapter.call (Executors.java:511)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.ThreadPoolExecutor.runWorker (ThreadPoolExecutor.java:1142)
    at java.util.concurrent.ThreadPoolExecutor$Worker.run (ThreadPoolExecutor.java:617)
    at java.lang.Thread.run (Thread.java:745)
Caused by: org.apache.maven.doxia.siterenderer.RendererException: Cannot use skin: has 1.7.1 Doxia Sitetools prerequisite, but current is 1.7
    at org.apache.maven.doxia.siterenderer.DefaultSiteRenderer.createContextForSkin (DefaultSiteRenderer.java:811)
    at org.apache.maven.plugins.site.render.AbstractSiteRenderingMojo.createSiteRenderingContext (AbstractSiteRenderingMojo.java:327)
    at org.apache.maven.plugins.site.run.SiteRunMojo.createWebApplication (SiteRunMojo.java:179)
    at org.apache.maven.plugins.site.run.SiteRunMojo.execute (SiteRunMojo.java:87)
    at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo (DefaultBuildPluginManager.java:134)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:209)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:155)
    at org.apache.maven.lifecycle.internal.MojoExecutor.execute (MojoExecutor.java:147)
    at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject (LifecycleModuleBuilder.java:116)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:185)
    at org.apache.maven.lifecycle.internal.builder.multithreaded.MultiThreadedBuilder$1.call (MultiThreadedBuilder.java:181)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.Executors$RunnableAdapter.call (Executors.java:511)
    at java.util.concurrent.FutureTask.run (FutureTask.java:266)
    at java.util.concurrent.ThreadPoolExecutor.runWorker (ThreadPoolExecutor.java:1142)
    at java.util.concurrent.ThreadPoolExecutor$Worker.run (ThreadPoolExecutor.java:617)
    at java.lang.Thread.run (Thread.java:745)
[ERROR] 
[ERROR] Re-run Maven using the -X switch to enable full debug logging.
[ERROR] 
[ERROR] For more information about the errors and possible solutions, please read the following articles:
[ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoExecutionException
