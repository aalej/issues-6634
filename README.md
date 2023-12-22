# Repro for Firebase Tools issue 6634 (TypeScript)

### Environment Info

- firebase-tools: v13.0.2 and v12.9.0<br>
- node: v20.10.0

### Steps to reproduce

1. Run `firebase deploy --project <project_id> --force`
1. Wait for deployment to complete
1. Re-run `firebase deploy --project <project_id> --force`
1. Outputs the ff:

```
✔  functions[api-func1Api(us-central1)] Skipped (No changes detected)
✔  functions[api-func2Api(us-central1)] Skipped (No changes detected)
```
