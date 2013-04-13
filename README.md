ASP.NET MVC Versions
=================

This is a collection of out-of-the-box ASP.NET MVC project versions.

The ultimate goal is to determine how things have actually changed between versions, to both ease the upgrade path and determine how to revert back, if necessary.

Method
---

1. All supported Visual Studio 2010 SP1 ASP.NET MVC projects were created fresh. This covered versions 1-2, as well as the Empty, Internet, and Intranet project templates for version 3.
2. Visual Studio 2012 was used to create projects covering version 3 (Empty, Internet, and Intranet).
3. Visual Studio 2012 was used to create projects covering version 4 (Basic, Internet, Intranet, Mobile, and Web API).
4. Another machine, with Visual Studio 2012 Update 1 was used to create projects covering version 3 (Empty, Internet, and Intranet). There was one change, noted below.
5. That same machine was used to create projects covering version 4 (Basic, Internet, Intranet, Mobile, and Web API).
6. Visual Studio 2012 Update 2 was used to create a new project using the MVC 3 Internet project template and no changes were found.
7. Visual Studio 2012 Update 2 was used to create projects covering version 4 (Basic, Internet, Intranet, Mobile, and Web API).

Visual Studio 2010 SP1 to 2012 differences
---

TODO

Visual Studio 2012 to Update 1 differences
---

1. Visual Studio 2012 and Visual Studio 2012 Update 1 have no real changes to the ASP.NET MVC 3 projects, with the exception of the following code, added immediately before the system.web sessionState element in the root Web.config:

    <!--
            If you are deploying to a cloud environment that has multiple web server instances,
            you should change session state mode from "InProc" to "Custom". In addition,
            change the connection string named "DefaultConnection" to connect to an instance
            of SQL Server (including SQL Azure and SQL  Compact) instead of to SQL Server Express.
      -->

TODO

Visual Studio 2012 Update 1 to Update 2 differences
---

1. MVC 3 templates do not appear to have changed. Only the Internet template was tested.
2. MVC 4 templates use jQuery UI 1.8.24 instead of jQuery UI 1.9.2. I've found no information on why this change was made. 
