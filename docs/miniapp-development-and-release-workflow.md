# Mini-App Development and Release Workflow

Every mini-app change is complete only after the full cycle below is complete.

## 1. Problem and scope

- State the repeated field-work situation that motivated the app.
- Record the existing manual process, its slow or error-prone steps, and the exact outcome the app should produce.
- Keep the first release focused on one workflow.

## 2. Specification and implementation

- Define accepted input formats, output format, ambiguous-input rules, and error behavior.
- Build the smallest interface that completes the workflow quickly.
- Include repeat-work details such as automatic next-entry preparation, one-tap clear, and help that stays out of the normal flow.

## 3. Device validation

- Test the primary happy-path inputs and invalid inputs.
- Test on the actual target phone, both with the keyboard closed and with the numeric keyboard open.
- Check system-bar safe areas, camera cutouts, navigation areas, and the position of the primary result.
- Record any observed UI problem as a GitHub Issue with: screenshot/context, cause, resolution, version, and remaining verification steps.

## 4. Release

- Increase `versionCode` and `versionName` for every installable update.
- Build and verify the APK version before publishing it.
- Publish a GitHub Release with the APK attached and short user-facing release notes.

## 5. Documentation and publication

- Update the README with behavior changes and the version change log.
- Update specification or workflow documentation when a rule, layout decision, or validation practice changes.
- Link resolved implementation work to its relevant GitHub Issue; close the issue only after the fix is verified on the target device.
- Confirm the repository contains the source, README, release notes, and downloadable APK before calling the update complete.

## Completion checklist

- [ ] Problem and scope documented
- [ ] Feature implemented
- [ ] Actual-device behavior checked
- [ ] UI issues recorded and tracked
- [ ] Version incremented
- [ ] APK built and version verified
- [ ] GitHub Release published with APK
- [ ] README and technical notes updated

