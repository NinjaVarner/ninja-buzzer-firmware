# Local signed firmware release candidate

Not published. Hardware qualification is still in progress; do not merge/push
this candidate into public main until all required MCU/phone checks pass.

Only the authentic 1.5.1 candidate is staged here. The intentional 1.5.2 startup
fault test image and recovery backups must never be distributed.

Existing legacy releases remain unchanged. Public app minimum versionCode is79
(planned APK V3.10), package com.ninjabuzzers.timer. Protocol1 devices require
a one-time, recovery-backed USB migration before accepting signed protocol2 OTA.

Pinned publisher SPKI SHA256:
604ae11c91d278afb9f55b1dc9d5617fa5d38109a3461386a492cba9da7447ca

Candidate image SHA256:
53293bdfefbaab157fb9c8929c695b41a85107b2c32042a4af65cce2de3d2e24

The dedicated manifest-qa.json targets pre-release QA app code78 and raw
HTTPS files on this candidate branch. The production manifest retains minimum
code79. Live GitHub Pages/main are unchanged until explicitly published.
