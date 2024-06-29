# Jupyter Notebook Template

This is a template that can be used to share Python code between your Jupyter Notebooks.

## Autoreload Extension

If you are using VS Code, you can setup the autoreload extension globally to reload modules when cells are executed.
That way you don't have to restart the Python kernel when code in the shared package has changed.
Add the following setting to your user `settings.json`.

```
{
    ...
    "jupyter.runStartupCommands": [
        "%load_ext autoreload",
        "%autoreload 2"
    ]
}
```

If you cannot specify these commands to run at the startup of the notebooks, you have to add these two lines to every notebook if you want the autoreald extension.

```
%load_ext autoreload
%autoreload 2
```