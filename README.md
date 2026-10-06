# Mapp — Android beta

Mapp is a personal mobile health record. It runs **entirely offline**: no
internet connection, no account, and no data ever leaves the phone.

This repository exists only to hand out builds. There is no source code here.

## Install

1. Open the [Releases page](../../releases) on the phone.
2. Download **`Mapp-<version>-universal.apk`**.
3. Open the downloaded file (the browser offers this, or use the phone's
   Files app).
4. Android will say the file is from an unknown source. Allow *install
   unknown apps* for the app that is opening it. **You only do this once.**
5. Tap **Install**, then **Open**.

### Which file?

| File | Use it when |
|---|---|
| `universal` | Always works. Start here. |
| `arm64` | You want a smaller download. Fits most phones from 2016 on. |
| `arm32` | Older or low-end phones that reject `arm64`. |

If `arm64` or `arm32` refuses to install, use `universal`.

### Checking the download (optional)

Each release includes `Mapp-<version>-SHA256SUMS.txt`. On a computer:

```sh
shasum -a 256 -c Mapp-<version>-SHA256SUMS.txt
```

## First start

1. Mapp asks the phone's owner to register: name, gender, date of birth,
   address, an identifier such as a national ID, insurance details, and a
   calendar color.
2. You choose an **app password**. It unlocks the app every time and
   protects every record on the phone. It cannot be reset — choose one you
   will remember.
3. You also choose a **recovery key**. This is a separate family secret, and
   it is the only way your records can be restored onto a new phone if this
   one is lost, broken or wiped. Your clinician needs it to do that restore.
   Write it down and keep it somewhere other than the phone.
4. Family members can be added afterwards from the Home screen.

Every later start asks for that password, or a fingerprint / face unlock once
the phone offers it.

## Being told about new versions

New releases are announced on the **mHealth-Africa** channel on WhatsApp:

<https://whatsapp.com/channel/0029VbEKtorEVccSIbVooe0L>

Follow it and you get a message whenever a new Dapp or Mapp is out. It is
one-way — you cannot reply there, and no one sees who else follows it.

## Notes

- These are **beta** builds. Expect rough edges, and report anything odd to
  whoever gave you this link.
- Updates are not automatic. New versions appear on the releases page.
- Installing a new version keeps your existing records. Uninstalling Mapp
  deletes them.
