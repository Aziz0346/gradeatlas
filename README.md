# GradeAtlas MCP

GradeAtlas MCP — convert grades between 1,159 grading systems across 246 countries into the US 4.0 GPA scale, with university search and country grading guides.

## MCP endpoint

Remote MCP server (Streamable HTTP, no authentication required):

```
https://zhitmyoghxfwqcprrqjf.supabase.co/functions/v1/mcp
```

Add the URL above as a remote MCP server in Claude, ChatGPT, Cursor, or any MCP client that supports Streamable HTTP servers. More on https://gradeatlas.org.

## Tools

The server exposes 12 tools: `convert_grade`, `get_us_equivalent`, `gpa_to_percentage`, `calculate_gpa`, `resolve_grading_scale`, `list_countries`, `get_country_grading_systems`, `get_grade_mappings`, `search_universities`, `get_institution`, `calculate_normalized_gpa`, and `get_country_guide`.

## Registry

This repository publishes the server to the [official MCP Registry](https://registry.modelcontextprotocol.io) as `io.github.Aziz0346/gradeatlas`. Publishing is automated: pushing a tag like `v0.1.0` runs the workflow in `.github/workflows/publish-mcp.yml`.

## License

MIT
