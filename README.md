# Legal documents

These Markdown files are plain-text copies of the documents shown inside the
app (Settings → Privacy Policy, Terms & Legal). They are generated from
`BrightNumbers/Legal/LegalDocuments.swift` with the values in
`BrightNumbers/Legal/LegalInfo.swift`.

Before submitting to the App Store:

1. Edit `LegalInfo.swift` (owner name, contact email, mailing address,
   privacy and terms URLs, governing law state, venue, date).
2. Hosting: these files live in the public repo https://github.com/DefDamian/Brightnumbers
   (root level, branch `main`). Whenever you change `LegalDocuments.swift`,
   push the regenerated .md files there too so the app and the web copy match.
   Privacy Policy URL for App Store Connect:
   `https://github.com/DefDamian/Brightnumbers/blob/main/PRIVACY-POLICY.md`
3. In App Store Connect → App Privacy, answer "Data Not Collected".
4. Pick the Kids Category age band and confirm no third-party ads/analytics.
5. Host `TERMS-OF-USE.md` at the URL in `LegalInfo.termsURL` and paste it into
   App Store Connect → App Information → License Agreement (custom EULA),
   or leave Apple's standard EULA; either is fine since the in-app acceptance
   screen already binds the user to these Terms.
6. Whenever you change the Terms or Privacy Policy, bump `LegalInfo.termsVersion`
   so existing users are asked to accept the new version.
