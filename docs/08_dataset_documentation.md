# 08 — Dataset Documentation

## Primary Dataset — GTZAN Genre Collection

| Property | Detail |
|----------|--------|
| Tracks | 1,000 audio files |
| Duration | 30 seconds each |
| Genres | 10 (blues, classical, country, disco, |
|        | hiphop, jazz, metal, pop, reggae, rock) |
| Format | .wav, 22050 Hz, mono |
| Size | ~1.2 GB |
| Source | Kaggle / Marsyas website |
| Licence | Free for research use |

## Known Limitations
- Small dataset by modern standards
- Some mislabelled tracks reported in literature
- Western music only — limited cultural diversity

## Mitigation Strategy
- Data augmentation (pitch shift, time stretch, noise)
- Cross-validation to reduce mislabel impact
- Carnatic samples added manually as bonus extension

## Genre to Mood Mapping
| Genre | Mood State |
|-------|-----------|
| Classical | Calm |
| Jazz | Calm |
| Blues | Sad |
| Country | Sad |
| Metal | Energetic |
| Rock | Energetic |
| Hiphop | Energetic |
| Disco | Happy |
| Pop | Happy |
| Reggae | Happy |
