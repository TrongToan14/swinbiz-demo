# Bank Data Security Program (BDSP) – Demo

Interactive browser demo of the BDSP threat-detection pipeline. Simulated VPC Flow Logs and CloudTrail events stream in, detection rules flag suspicious behaviour, and alerts show the time to detect.

All data is generated in the browser. No AWS account or backend is needed.

## Run locally

Open `index.html` in any browser.

## Detection rules

- Port scan: 12+ distinct ports from one source in 10 s
- SSH brute force: 6+ rejected SSH attempts from one source in 10 s
- Data exfiltration: single outbound flow over 500 MB to an external IP
- Root console login without MFA
- AdministratorAccess attached to a user
- CloudTrail logging stopped
- Console login from a new IP (review only)

## Live site

After enabling GitHub Pages, the demo is at `https://<your-username>.github.io/<repo-name>/`.
