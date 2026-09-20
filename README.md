# oci-arm-hunt

Unattended Always Free Ampere A1 (`VM.Standard.A1.Flex`) hunter for tenancy `fawxyz` / `ap-kulai-2`.

Retries every 10 minutes until `penrose` launches. Capacity errors are expected. Disable this workflow after success.

## Spec
- Shape: 2 OCPU / 12 GB (Always Free max as of 2026-06)
- Image: Canonical Ubuntu 24.04 aarch64
- Boot: 200 GB balanced
- Subnet: existing `penrose-vcn` public subnet
- Region: Malaysia West 2 (`ap-kulai-2`), AD-1 only

## Secrets required
See `.github/workflows/hunt.yml` env block / repo Settings → Secrets.
