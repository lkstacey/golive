```mermaid
graph TD
    A[Start] --> B{SPoA team receives referral};

    B --> C{Can SPoA team process referral and schedule Dora call?};

    C -- Yes --> D[SPoA team processes referral and schedules Dora call];
    D --> E[Receive email confirmation within 2 working days];
    E --> F[End];

    C -- No --> G{Inability to process due to patient details?};

    G -- Yes --> H[SPoA team emails requesting patient detail check];
    H --> I[Email subject: &#91;ACTION REQUIRED&#93;];
    I --> J[You check/confirm patient details against GP records];
    J --> K[You resend updated referral to SPoA team];

    K --> L{SPoA team receives correct patient details within 5 working days?};

    L -- Yes --> D;
    L -- No --> M[Referral rejected];
    M --> F;
```
