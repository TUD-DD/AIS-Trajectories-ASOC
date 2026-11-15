# AIS Vessel Trajectory Data

The data are stored in Excel (`.xlsx`) format. Each file contains one trajectory, and each row represents one AIS observation. The worksheet is named `Trajectory`.

## Time Range

The following range applies to the globally compressed timestamps, in UTC:

- Start: **2024-04-01 00:00:00**
- End: **2024-06-30 23:59:59**

## Archive Password

For the password-protected data archive, use the **manuscript ID of the associated paper** as the extraction password. Enter the complete ID exactly as assigned, including letters, numbers, and hyphens. The password is case-sensitive.

## File Naming

```text
Trajectory_<trajectory_id>_MMSI_<vessel_mmsi>.xlsx
```

Example: `Trajectory_0001_MMSI_209287000.xlsx`. A vessel may have multiple trajectory files.

## Data Fields

| Field | Description | Format or unit |
|---|---|---|
| `TrajectoryID` | Trajectory identifier | Integer |
| `MMSI` | Maritime Mobile Service Identity | Nine-digit integer |
| `BaseDateTime` | UTC timestamp as text | `yyyy-MM-dd HH:mm:ss.SSSSSS` |
| `LAT` | Latitude | Degrees |
| `LON` | Longitude | Degrees |
| `SOG` | Original speed over ground, unchanged by time compression | Knots |
| `COG` | Course over ground | Degrees |
| `Heading` | Vessel heading | Original source encoding retained |
