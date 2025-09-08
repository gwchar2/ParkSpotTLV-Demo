# ParkSpotTLV
<!-- Status & releases -->
![Build](https://img.shields.io/github/actions/workflow/status/gwchar2/ParkSpotTLV-Demo/ci.yml?label=Build%20%2B%20Tests)
![Latest release](https://img.shields.io/github/v/release/gwchar2/ParkSpotTLV-Demo?display_name=tag&sort=semver)
![Release date](https://img.shields.io/github/release-date/gwchar2/ParkSpotTLV-Demo)


## Example commit messages
Triggers a release (and what it bumps)
feat: → MINOR, fix: → PATCH, feat!: or BREAKING CHANGE: → MAJOR.

MINOR:
```feat: add parking zone overlay to map```

PATCH:
```fix: handle null permit when decoding jwt```

MAJOR (breaking):
```feat!: switch auth scheme to Bearer```
(or any commit with a footer BREAKING CHANGE: details_here)

## Does NOT trigger a release

```chore: rename solution folders```

```docs: update readme badges```

```ci: bump actions/checkout to v4```

```test: add unit tests for permits service```


## Project Structure
```
ParkSpotTLV/
├─ BackEnd/
│  └─ ParkSpotTLV.Api/
│     ├─ Config/
│     ├─ Data/               # DbContext + Migrations/
│     ├─ Endpoints/
│     ├─ Entities/
│     ├─ Infrastructure/
│     ├─ Seed/
│     ├─ appsettings*.json
│     └─ ParkSpotTLV.Api.csproj
│
├─ MobileApp/
│  └─ ParkSpotTLV.App/
│     ├─ Models/
│     ├─ Pages/
│     ├─ Platforms/
│     ├─ Resources/
│     ├─ Services/
│     ├─ ViewModels/
│     └─ ParkSpotTLV.App.csproj
│
├─ Shared/
│  └─ ParkSpotTLV.Contracts/
│     └─ ParkSpotTLV.Contracts.csproj
│
├─ Tests/
│  └─ .gitkeep               # (add test projects later)
│
├─ Database/
│  └─ .gitkeep               # seed data / local snapshots (optional)
│
├─ .github/
│  └─ workflows/
│     └─ ci.yml
│
├─ ParkSpotTLV.sln
├─ README.md
├─ .gitignore
└─ .gitattributes
```