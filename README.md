Save and switch named OAuth accounts for Pi's built-in providers.
Each Pi session keeps its own selection for every provider, and choosing `default` restores Pi's normal authentication only for that session without deleting saved accounts.

Active OAuth-only bridge providers stay visible while Pi resolves its initial scoped or saved default model, and fail closed if runtime authentication cannot be restored.
