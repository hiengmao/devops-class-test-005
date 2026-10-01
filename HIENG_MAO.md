# DevOps Conception Class
- Student: HIENG MAO

## Lesson 2: My CI/CD pipeline

### Welcome app: pipeline design
- Project: Flutter welcome screen + Laravel GET /welcome
- Trigger: push to practice branch
- Target: Laravel staging server + Android test device
### Stage: action | owner | output | mode
1. Code: commit API + screen | developer | commit | manual
2. Test: check API + screen | developer | test results | automatic
3. Build: package API + APK | developer | artifacts | automatic
4. Release: approve v1.0.0 | release lead | approved version | manual
5. Deploy: stage API; install APK | ops/tester | running app | manual
### Controls
Test/build fails: stop release; fix the code and rerun checks.
Release approval: release lead checks results and artifacts.
After deploy: open the app and confirm the welcome message appears.
If the check fails: stop rollout; restore the last working version.
Feedback: text is too small; create an issue to improve the screen.
