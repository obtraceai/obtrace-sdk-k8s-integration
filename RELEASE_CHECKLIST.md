# Release Checklist

- Validate Helm chart templates:
  - `helm template obtrace-sdk-integration ./chart >/tmp/obtrace-sdk-k8s-render.yaml`
- Validate example manifest:
  - `kubectl apply --dry-run=client -f ./obtrace-sdk.example.yaml`
- Verify values files:
  - `chart/values.yaml`
  - `chart/values-dev.yaml`
  - `chart/values-prod.yaml`
- Update README if chart values changed.
- Tag and release.
