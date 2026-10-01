Save and switch named OAuth accounts for Pi's built-in providers.
Each Pi session keeps its own selection for every provider, and choosing `default` restores Pi's normal authentication only for that session without deleting saved accounts.

Active OAuth-only bridge providers stay visible while Pi resolves its initial scoped or saved default model, and fail closed if runtime authentication cannot be restored.

## Startup default accounts

Open `/accounts` → **Startup default accounts**, then select a saved account to
turn its startup default **on** or **off**. A `✓` marks the enabled account; `○`
marks an account that is off. Each provider has at most one startup default, so
turning one account on replaces that provider's previous default. Turning the
current default off makes new sessions use the provider's normal Pi login.

The main menu shows **Active accounts (this session)** separately from
**Startup defaults (new sessions)**. Changing a startup default does not switch
any open session, rewrite resumed sessions, or delete saved credentials. Use the
existing **Switch … account** action to change only the current session.

The preference uses the existing provider `active` field in `pi-accounts.json`;
no migration or account re-login is required.
