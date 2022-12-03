# test-cosign-keyless-aqua-installer

Keyless Signing with [Cosign](https://docs.sigstore.dev/cosign/overview)

- https://github.com/suzuki-shunsuke/test-cosign-keyless-aqua-installer/releases/tag/v0.1.0-4
- https://github.com/suzuki-shunsuke/test-cosign-keyless-aqua-installer/blob/main/.github/workflows/release.yaml

## Verify

```console
$ COSIGN_EXPERIMENTAL=1 cosign verify-blob \
    --signature https://github.com/suzuki-shunsuke/test-cosign-keyless-aqua-installer/releases/download/v0.1.0-4/aqua-installer.sig \
    --certificate https://github.com/suzuki-shunsuke/test-cosign-keyless-aqua-installer/releases/download/v0.1.0-4/aqua-installer.pem \
    aqua-installer
tlog entry verified with uuid: 57d74bfb9371f19a4920717517ee436aa6cf3b1a914429723763026119292030 index: 8355170
Verified OK
```

## LICENSE

[MIT](LICENSE)
