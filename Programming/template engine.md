A **template engine** is a tool that takes a template—usually HTML—and fills it with [[dynamic data]] from your program.

For example,

```python
name = "Ernest"
```

Python gives the subject a value: Ernest

```HTML
<h1>Hello {{ name }}</h1>
```
and HTML receive the value from the same subject "name"

The engine that combines these two is Jinja by default for flask

Other template Engines:
- **Django Template Language ([[DTL]])** — built into [[Django]].
- **[[Mako]]** — Python-based and more permissive about embedding Python-like logic.
- **[[Chameleon]]** — often used with Pyramid; focuses on HTML/XML templates.
- **[[Mustache]]** — a simpler, logic-light templating system available in many languages.
- **[[Handlebars]]** — similar to Mustache, more common in JavaScript.

---
## Clarification

> [Distinction between template and template engine]
> Jinja              → template engine
> home.html           → template
> 
> Django Templates    → template engine
> dashboard.html       → template

Example of architecture 
project/
├── app.py
└── templates/
    ├── index.html
    ├── dashboard.html
    ├── simulation.html
    ├── results.html
    └── base.html