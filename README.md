# wpftxtest1

important commands

`winrm e winrm/config/listener`

`New-SelfSignedCertificate -DnsName WhateverTargetMachineAddressYouNeed -CertStoreLocation Cert:\LocalMachine\My`


`winrm delete winrm/config/listener?Address=*+Transport=HTTPS`

`winrm create winrm/config/listener?Address=*+Transport=HTTPS @{Hostname="WhateverTargetMachineAddressYouNeed";CertificateThumbprint="TheThumbprintYouCopied";port="5986"}`
