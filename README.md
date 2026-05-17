# MyCrew Unity Templates

Per-template checkouts used by MyCrew's project scaffolding flow.
Cloned by `backend/services/template_cloner_svc.py` when a user kicks
off a new project; the chosen subfolder is copied into the user's
chosen root directory and renamed to the project's English name.

## Layout

| Subdir          | Maps to template_id     |
|-----------------|-------------------------|
| `Universal2D/`  | `unity_universal_2d`    |
| `Universal3D/`  | `unity_universal_3d`    |
| `ARMobile/`     | `unity_ar_mobile`       |
| `MRCore/`       | `unity_mr_core`         |

Each subdir is a stripped Unity project: Assets/, Packages/,
ProjectSettings/. Unity regenerates Library/, Logs/, Temp/, obj/,
.csproj/.sln, and UserSettings/ on first editor open, so none of
those are committed here.
