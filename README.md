# Microsoft.KMS 10.0.0.6

## [Download Here][Download]

[Download]: https://github.com/thekevinholman/Microsoft.KMS/archive/refs/heads/main.zip

### Microsoft Key Management Service (KMS) Management Pack  
### This MP supports KMS on Windows Server 2012 R2 and later

Discovers and Monitors:
* KMS Servers

Key Monitoring Scenarios:
* KMS Service
* Idle Minutes Count
* Low Activation Count
* Initialization Failures
* DNS Failures

Troubleshooting:  The primary method of discovery is to search for a registry value "KeyManagementServiceListeningPort" in the following registry key:  "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\SoftwareProtectionPlatform\"  If your KMS is not getting discovered - you can add that registry value.  The default is REG_SZ with "1688"

History:
* 10.0.0.5 - Original release
* 10.0.0.6 - Modified discovery to ONLY search for registry value: "KeyManagementServiceListeningPort" at key: "HKLM\SOFTWARE\Microsoft\Windows NT\CurrentVersion\SoftwareProtectionPlatform\"
