# EyeSafe — Distribution channel

Public, binary‑only distribution for the **EyeSafe** Android app (source is private).
Each GitHub Release here contains the signed APKs and a `latest.json` manifest that
the app's built‑in **Check for updates** feature reads.

- Verify any APK is genuine: it must be signed by `CN=EyeSafe`
  (SHA‑256 `B7:A1:D1:04:5E:24:A9:64:3A:2D:1E:3A:AB:B6:39:51:75:58:B2:92:5A:59:56:42:81:68:DC:9B:78:17:0E:07`).
- Not a medical device.

## Android install troubleshooting

If Android says you must disable advanced security before installing, this is usually
Play Protect / device security blocking sideloaded APKs.

1. Download the APK from this repository's **Releases** page.
2. Open it and allow installs from the app you used to download it (browser/files app)
   when prompted (**Install unknown apps**).
3. If you see a Play Protect warning, choose **More details** and continue only if the
   signing fingerprint matches the one above.
4. If your device enforces **Advanced Protection** or managed security policy, APK
   sideloading can be blocked entirely. In that case, installation is not possible
   until that policy is changed.

### Child account note (Family Link / supervised devices)

Child accounts can block unknown app installs by policy, and the child cannot override
that setting. A parent/guardian must approve or change the Family Link/device policy
before EyeSafe can be installed from APK.
