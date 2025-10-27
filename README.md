# ARMSX2 Compatibility List

Welcome to the official ARMSX2 compatibility database! This repository contains community-maintained compatibility information for games running on ARMSX2.

## How to Contribute

To submit your updated compatibility lists:

1. **Fork this repository**
2. **Update the `compatibility.json` file** with your game compatibility data
3. **Submit a Pull Request** with your changes
4. **Wait for approval** - We will review and approve your changes once everything looks good

## Required JSON Format

All compatibility entries **must** follow this exact format with all mandatory fields, for example:

```json
{
  "games": [
    {
      "title": "Final Fantasy X",
      "status": "Perfect",
      "title-id": "SLUS-20312",
      "notes": "Runs at full speed with no graphical issues",
      "region": "NTSC-U",
      "tested_socs": ["SD 888"]
    },
    {
      "title": "Kingdom Hearts",
      "status": "Playable",
      "title-id": "SLES-51234",
      "notes": "Minor audio glitches in cutscenes",
      "region": "PAL-E",
      "tested_socs": ["SD 888"]
    },
    {
      "title": "Metal Gear Solid 2",
      "status": "In-Game",
      "title-id": "SLUS-20312",
      "notes": "Some graphical glitches in certain areas",
      "region": "NTSC-J",
      "tested_socs": ["SD 888"]
    }
  ]
}
```

## Mandatory Fields

Each game entry **must** include all of the following fields:

| Field | Description | Example |
|-------|-------------|---------|
| `title` | The official game title | `"Final Fantasy X"` |
| `status` | Compatibility status (see status guide below) | `"Perfect"` |
| `title-id` | The game's title ID from the disc | `"SLUS-20312"` |
| `notes` | Detailed compatibility notes | `"Runs at full speed with no graphical issues"` |
| `region` | Game region | `"NTSC-U"`, `"PAL-E"`, `"PAL-A"`, `"NTSC-J"` |

## Status Guide

Use one of these exact status values:

- **Perfect** - Game runs flawlessly with no issues
- **Playable** - Game is fully playable with minor issues
- **In-Game** - Game boots and runs but has significant issues
- **Menu** - Game boots to menu but crashes or fails in-game
- **Broken** - Game fails to boot or immediately crashes

## Region Codes

Use these standard region codes:

- **NTSC-U** - North America
- **PAL-E** - Europe
- **PAL-A** - Australia
- **NTSC-J** - Japan
- **NTSC-K** - Korea
- **NTSC-C** - China

## Submission Guidelines

- Ensure all mandatory fields are present and correctly formatted
- Use accurate and descriptive notes about compatibility
- Test games thoroughly before submitting
- One game entry per ID ensure the game you are testing for doesnt exist and if so why we should overwrite it
- Include any specific settings or configurations used

Thank you for contributing to the ARMSX2 compatibility database!