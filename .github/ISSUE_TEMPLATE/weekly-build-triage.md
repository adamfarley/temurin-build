---
name: :hospital: Weekly Build Triage
about: For triaging the nightly and weekend build failures
title: 'Weekly build triage for the week starting <YYYY>/<MM>/<DD>'
labels: 'weekly-build-triage'
---

This issue template is designed to create a consistent table of results that people can consult at-a-glance to get a sense of
how the builds 

| Date       | Day     | JDK Version | Pipeline | Pass/Build Fail/Test Fail | Triage Status            | Triager | Breakdown    |
| ---------- | ------- | ----------- | -------- | ------------------------- | ------------------------ | ------- | ------------ |
| 2023/03/31 | E.G.day | JDKnn       | Link     | 50/3/19                   | Pending/In Progress/Done | Grogu   | Comment Link |

Note: "Test_Fail" is for when all the "build" jobs passed (build, sign, installer, etc) but one of the test jobs failed and the
      status propagated upstream to the build job. Note that "unstable" test job status can be considered a pass, as these are 
      commonly unit tests that have failed for reasons unconnected to the build process itself.


Comment template:

Triage breakdown for \<Pipeline link\>

Table of failures:

\| Build Fail\/Test Fail \| Platform   \| Failed Job \| Response                              \| Issue \| Triage Status              \| Notes  \|
\| --------------------- \| ---------- \| ---------- \| ------------------------------------- \| ----- \| -------------------------- \| -----  \|
\| Build Fail\/Test Fail \| e.g. win64 \| Link       \| Raise (Issue)/Existing (Issue)/Ignore \| Link  \| Pending\/In Progress\/Done \| Borked \|