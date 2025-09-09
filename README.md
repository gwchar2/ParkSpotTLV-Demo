# ParkSpotTLV
<!-- Status & releases -->
![Build](https://img.shields.io/github/actions/workflow/status/gwchar2/ParkSpotTLV-Demo/ci.yml?branch=master&label=Build%20%2B%20Tests)
![Latest release](https://img.shields.io/github/v/release/gwchar2/ParkSpotTLV-Demo?display_name=tag&sort=semver)
![Release date](https://img.shields.io/github/release-date/gwchar2/ParkSpotTLV-Demo)


## Example commit messages
The following triggers a release (and what it bumps)
fix: → PATCH; 
feat: → MINOR; 
feat!: or BREAKING CHANGE: → MAJOR;

### PATCH (v0.0.1 → v0.0.2):

```fix: handle null permit in auth middleware```

```fix: correct DTO mapping for ParkingSpot```

### MINOR (v0.0.x → v0.1.0):

```feat: add parking zones overlay to map```

```feat: expose /api/permits endpoint```

### MAJOR (v0.x.y → v1.0.0) — breaking change:

```feat!: switch authentication to Bearer tokens```

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