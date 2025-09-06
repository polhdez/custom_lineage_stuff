For creating the keys follow:

https://wiki.lineageos.org/signing_builds/

For creating releasekey.key for avb: 
`openssl pkcs8 -in releasekey.pk8 -inform DER -out releasekey.key -nocrypt`

Store the keys on `~/.android-certs` and symlink to your lineageos build dir like `ln -s ~/.android-certs/ ~/android/lineage/android-certs` so the build script can access them for creating vbmeta
