[QUARTZ](https://www.quartz-scheduler.net/)

    By default IIS recycles and stops app pools from time to time. This means that even if you have Application_Start event to start Quartz when web app is being first accessed, the scheduler might get disposed later on due to site inactivity.

    If you have a IIS 8 available, you can configure your site to be preloaded and kept running. See this blog post for details.
