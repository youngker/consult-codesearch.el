consult interface for codesearch

## Requirements

- **Google codesearch**

  [https://github.com/google/codesearch](https://github.com/google/codesearch)


You can add these lines to your init file.

```elisp
(use-package consult-codesearch
  :bind
  (("C-c h f" . consult-codesearch-find-file)
   ("C-c h t" . consult-codesearch)
   ("C-c h I" . consult-codesearch-build-index)
   :map minibuffer-local-map
   ("C-c h" . consult-history)
   ("C-c s" . embark-export)))
```

## Key bindings

Key | Function
--- | --------
<kbd>C-c h</kbd> | consult-history
<kbd>C-c s</kbd> | embark-export
