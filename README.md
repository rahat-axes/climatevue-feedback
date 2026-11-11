Collect user feedback, bug reports for https://climatevue-dev.gokyostudio.workers.dev/

# ClimateVue Issues & Feedback Tracker

Welcome to the community feedback and issue tracker for **ClimateVue**!

ClimateVue is a zero-setup, zero-cost platform that allows you to generate ready-made JAX-built notebooks, run climate forecasts on your own hardware (Google Colab, Kaggle, or local GPUs/TPUs), and upload a lightweight `results.zip` to visualize performance charts and logs.

To protect our codebase, this repository contains **no source code**. It is strictly a dedicated space for users to report bugs, ask questions, and suggest new features for the ClimateVue platform.

---

## 🛠️ How to Report Issues

Before opening a new issue, please **search the existing issues** to make sure someone else hasn't already reported the same problem.

When you are ready to submit, click on the **Issues** tab and choose one of our templates:

* **🐛 Bug Report:** Use this if a notebook fails to compile, an upload gets rejected incorrectly, or the dashboard charts display incorrect data.
* **💡 Feature Request:** Use this to suggest new climate models, support for additional GPU/TPU accelerators, or new visualization metrics on the dashboard.
* **❓ General Question:** Use this if you need help troubleshooting JAX environments or understanding your run diagnostics.

---

## 🧠 Common Troubleshooting Tips

Before filing a bug, check if your issue is covered by these common platform behaviors:

* **TPU Compilation Times:** Notebook compilation takes longer on TPUs than on GPUs. If your notebook feels stuck during the first cell, give it a few minutes.
* **Import Errors (TPU):** Do *not* manually `import jax` on a TPU platform. The notebook is pre-configured to manage JAX processes automatically.
* **Rejected Uploads:** If the browser rejects your `results.zip`, check the error message. It will call out the exact file causing the issue. Do not rename or repackage the zip file manually.
* **Lost Run Links:** Run IDs are randomized and entirely private—there is no public directory. Make sure to bookmark your dashboard URL immediately, as we cannot recover lost links for you.

---

## 🔒 Privacy & Security

ClimateVue is built to be secure and private by design:
* **No Accounts:** The platform requires no sign-up or login credentials.
* **Data Isolation:** Only the small configuration and metrics summary (~200 KB) inside `results.zip` is ever uploaded. Your raw, full forecast data **never leaves your local machine or cloud runtime**.
* **Retention:** Uploaded runs are automatically deleted after **30 days**.

*If you discover a sensitive security vulnerability, please do not post it publicly here. Contact directly or use GitHub's private vulnerability reporting feature.*

---

## 🚀 Ready to Forecast?
If you just want to run a simulation, head directly over to the [ClimateVue Platform](https://workers.dev). Generating a custom notebook takes less than a minute.
