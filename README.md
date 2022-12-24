# supabase-env
Making it easier to work with multiple Supabase keys for multiple projects

Include `supabase-env` in your bash profile config (~/.profile or ~/.bash_profile) by adding something like this:

```
# Supabase Settings
export SUPABASE_CREDENTIAL_FILE=~/.supabase/credentials
export SUPABASE_PROFILE=default
. ~/bin/supabase-env
```

After that you can use it with: `supabase-switch profile_name`

By default it will load the `SUPABASE_PROFILE` profile at the shell initialization. Make sure you provide the correct `SUPABASE_CREDENTIAL_FILE` that you are using (~/.supabase/credentials).

Other useful commands are: 
 * `supabase-unset` to unset the supabase_env keys, 
 * `supabase-list` to list all the available profiles defined in your `SUPABASE_CREDENTIAL_FILE`
 * `supabase-who` will show the current loaded profile.