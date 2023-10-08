# Build&Deploy Android App

Hai una app react native e vuoi toglierti il pensiero di aggiornare il file gradle prima di ogni build?

Vorresti automatizzare il deploy sul Play Store?

Usa questa action

> Se SERVICE_ACCOUNT_JSON non è impostato upload faccio upload dell'artefatto

### Usage
```yml
uses: AndreaMolinari/actions/.github/workflows/craft-release.yml@test
with:
  alpha: true
  beta: false
secrets:
  KEYSTORE64: ${{ secrets.KEYSTORE64 }}
  ANDROID_KEY_PASSWORD: ${{ secrets.ANDROID_KEY_PASSWORD }}
  ANDROID_ALIAS: ${{ secrets.ANDROID_ALIAS }}
  ANDROID_ALIAS_PASS: ${{ secrets.ANDROID_ALIAS_PASS }}
  NPM_TOKEN: ${{ secrets.NPM_TOKEN }}
  SERVICE_ACCOUNT_JSON: ${{ secrets.SERVICE_ACCOUNT_JSON }}
```