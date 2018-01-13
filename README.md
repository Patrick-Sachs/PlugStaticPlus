# PlugStaticPlus

See the original plug for the full documentation: [https://github.com/elixir-plug/plug/blob/master/lib/plug/static.ex](plug/static.ex)

New features/changes made in this plug:
  * Support for index handling. Requesting e.g. "/my-dir" while "/my-dir/index.html" exists will serve the "index.html" file. Respects the :custom_types setting if a reroute is performed.
    The index files can be specified by using the :index option with either a list of strings or a single string. The default is ["index.html", "index.htm", "index.js", "index.json"]
  * Files can be served from the "/" directory. Will respect index definitions.