
# Log关键字
## pbap
```markdown
06-23 09:58:50.771  7999  8139 D PbapStateMachine: WaitingForAuth: currentDevice=BC:30:7E:33:F3:55, msg=broadcastConnectionState BC:30:7E:33:F3:55: 0->1
06-23 09:58:50.779  7999  8139 D PbapStateMachine: Connected: currentDevice=BC:30:7E:33:F3:55, msg=broadcastConnectionState BC:30:7E:33:F3:55: 1->2 //连接状态改变时会发广播
//download phonebook
06-23 09:58:50.794  7999  5088 D BluetoothPbapObexServer: onConnect(): uuid=[121, 97, 53, -16, -16, -59, 17, -40, 9, 102, 8, 0, 32, 12, -102, 102]
06-23 09:58:50.805  7999  5088 D BluetoothPbapObexServer: OnGet type is x-bt/phonebook; name is telecom/pb.vcf
06-23 09:58:50.806  7999  5088 V BluetoothPbapObexServer: download phonebook request
06-23 09:58:50.806  7999  5088 I BluetoothPbapObexServer: maxListCount=65535 listStartOffset=0 searchValue= searchAttr= needTag=1 vcard21=true order=vcardselector=[B@58e3294vcardselop=0
06-23 09:58:50.862  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:50.862  7999  5088 D BluetoothPbapObexServer: Need Phonebook size in response header.
06-23 09:58:50.862  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:50.862  7999  5088 D BluetoothPbapObexServer: Send back Phonebook size only, without body info! Size= 302
06-23 09:58:50.862  7999  5088 D BluetoothPbapObexServer: Push Header
06-23 09:58:50.862  7999  5088 D BluetoothPbapObexServer: javax.obex.HeaderSet@36cd13d
06-23 09:58:51.343  7999  5088 V BluetoothPbapObexServer: download phonebook request
06-23 09:58:51.343  7999  5088 I BluetoothPbapObexServer: maxListCount=100 listStartOffset=0 searchValue= searchAttr= needTag=1 vcard21=true order=vcardselector=[B@8f1e7d7vcardselop=0
06-23 09:58:51.355  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:51.355  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:51.355  7999  5088 D BluetoothPbapObexServer: pullPhonebook(): requestSize=100 startPoint=0 endPoint=99
06-23 09:58:52.406  7999  5088 V BluetoothPbapObexServer: download phonebook request
06-23 09:58:52.406  7999  5088 I BluetoothPbapObexServer: maxListCount=100 listStartOffset=100 searchValue= searchAttr= needTag=1 vcard21=true order=vcardselector=[B@aed68c4vcardselop=0
06-23 09:58:52.421  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:52.421  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:52.421  7999  5088 D BluetoothPbapObexServer: pullPhonebook(): requestSize=100 startPoint=100 endPoint=199
06-23 09:58:53.313  7999  5088 V BluetoothPbapObexServer: download phonebook request
06-23 09:58:53.314  7999  5088 I BluetoothPbapObexServer: maxListCount=100 listStartOffset=200 searchValue= searchAttr= needTag=1 vcard21=true order=vcardselector=[B@89983advcardselop=0
06-23 09:58:53.334  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:53.334  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:53.335  7999  5088 D BluetoothPbapObexServer: pullPhonebook(): requestSize=100 startPoint=200 endPoint=299
06-23 09:58:54.380  7999  5088 V BluetoothPbapObexServer: download phonebook request
06-23 09:58:54.380  7999  5088 I BluetoothPbapObexServer: maxListCount=2 listStartOffset=300 searchValue= searchAttr= needTag=1 vcard21=true order=vcardselector=[B@449f6e2vcardselop=0
06-23 09:58:54.394  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:54.394  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:54.394  7999  5088 D BluetoothPbapObexServer: pullPhonebook(): requestSize=2 startPoint=300 endPoint=301
06-23 09:58:54.412  7999  5088 V BluetoothPbapVcardManager: contactIdCursor size: 2
06-23 09:58:54.451  7999  5088 D BluetoothPbapObexServer: OnGet type is x-bt/phonebook; name is SIM1/telecom/pb.vcf
06-23 09:58:54.451  6100  6170 D _V_LGS_BasicSQL: writeDelay table = aaa, values = duration=0 analysisdate=1592877534445 lunchcount=1 start_time=1592877534440 event_id=204 event_label=20419 event_value={"PbapTag":"pbap_contact","PhoneBook":"PhoneBook","vCardSelct":"false","pbSize":"2","TransferTimeMs":"27.0","TransferPhoto":"true","vcardType":"2.1","log_from":"com.android.bluetooth","version_code":29,"version_name":"9.1","system_version":"PD1962_A_1.9.0","rom_version":"rom_11.0","android_version":"10","ro_vivo_internet_name":"vivo S6","ro_vivo_market_name":"vivo S6","ro_product_model":"V1962A"} end_time=1592877534440

06-23 09:58:50.887  7999  5088 D BluetoothPbapObexServer: OnGet type is x-bt/phonebook; name is telecom/och.vcf
06-23 09:58:50.911  7999  5088 V BluetoothPbapObexServer: download outgoing calls request
06-23 09:58:50.911  7999  5088 I BluetoothPbapObexServer: maxListCount=65535 listStartOffset=0 searchValue= searchAttr= needTag=3 vcard21=true order=vcardselector=[B@765e400vcardselop=0
06-23 09:58:50.925  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:50.926  7999  5088 D BluetoothPbapObexServer: Need Phonebook size in response header.
06-23 09:58:50.926  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:50.926  7999  5088 D BluetoothPbapObexServer: Send back Phonebook size only, without body info! Size= 2
06-23 09:58:50.926  7999  5088 D BluetoothPbapObexServer: Push Header
06-23 09:58:50.926  7999  5088 D BluetoothPbapObexServer: javax.obex.HeaderSet@9da4439

06-23 09:58:51.010  7999  5088 D BluetoothPbapObexServer: OnGet type is x-bt/phonebook; name is telecom/ich.vcf
06-23 09:58:51.042  7999  5088 V BluetoothPbapObexServer: download incoming calls request
06-23 09:58:51.042  7999  5088 I BluetoothPbapObexServer: maxListCount=65535 listStartOffset=0 searchValue= searchAttr= needTag=2 vcard21=true order=vcardselector=[B@d11eaf5vcardselop=0
06-23 09:58:51.074  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:51.074  7999  5088 D BluetoothPbapObexServer: Need Phonebook size in response header.
06-23 09:58:51.074  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:51.074  7999  5088 D BluetoothPbapObexServer: Send back Phonebook size only, without body info! Size= 0
06-23 09:58:51.074  7999  5088 D BluetoothPbapObexServer: Push Header
06-23 09:58:51.074  7999  5088 D BluetoothPbapObexServer: javax.obex.HeaderSet@4b5e08a

06-23 09:58:51.085  7999  5088 D BluetoothPbapObexServer: OnGet type is x-bt/phonebook; name is telecom/mch.vcf
06-23 09:58:51.096  7999  5088 V BluetoothPbapObexServer: download missed calls request
06-23 09:58:51.096  7999  5088 I BluetoothPbapObexServer: maxListCount=65535 listStartOffset=0 searchValue= searchAttr= needTag=4 vcard21=true order=vcardselector=[B@96d6fbvcardselop=0
06-23 09:58:51.099  7999  8082 D BluetoothPbapService: getConnectionState: BC:30:7E:33:F3:55
06-23 09:58:51.102  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 8
06-23 09:58:51.103  7999  5088 D BluetoothPbapObexServer: Need Phonebook size in response header.
06-23 09:58:51.109  7999  5088 D BluetoothPbapObexServer: handleAppParaForResponse(): mNeedNewMissedCallsNum=true,  num= 0
06-23 09:58:51.109  7999  5088 D BluetoothPbapObexServer: checkPbapFeatureSupport featureBitMask is 4
06-23 09:58:51.109  7999  5088 D BluetoothPbapObexServer: Send back Phonebook size only, without body info! Size= 0
06-23 09:58:51.109  7999  5088 D BluetoothPbapObexServer: Push Header
06-23 09:58:51.109  7999  5088 D BluetoothPbapObexServer: javax.obex.HeaderSet@6dc3318
```

## Map
```
06-23 09:58:54.898  7999  7999 D BluetoothMapService: onReceive: android.bluetooth.device.action.CONNECTION_ACCESS_REPLY
06-23 09:58:54.898  7999  7999 D BluetoothMapService: Received ACTION_CONNECTION_ACCESS_REPLY:3isWaitingAuthorization:true
06-23 09:58:54.898  7999  7999 D BluetoothMapService: cancelUserTimeOutAlarm()
06-23 09:58:54.903  7999  7999 D BluetoothMapService: setMessageAccessPermission(ACCESS_ALLOWED) result=true
06-23 09:58:54.904  7999  7999 D BluetoothPbapService: action: android.bluetooth.device.action.CONNECTION_ACCESS_REPLY
06-23 09:58:55.014  7999  7999 D BluetoothMapService: onReceive: android.bluetooth.device.action.SDP_RECORD
06-23 09:58:55.014  7999  7999 D BluetoothMapService: Received ACTION_SDP_RECORD.
06-23 09:58:55.035  7999  8130 D BluetoothMapService: mPermission = 1
06-23 09:58:55.035  7999  8130 D BluetoothMapService: Map Service START ObexServerSessions()
06-23 09:58:55.041  7999  8130 D BluetoothMapMasInstance0:     ServerSession started.
06-23 09:58:55.041  7999  8130 D BluetoothMapService: Map state 0 -> 2, result = 1
06-23 09:58:55.041  7999  5205 D BluetoothMapObexServer: onConnect():
06-23 09:58:55.041  7999  5205 D BluetoothMapObexServer: onConnect(): uuid=[-69, 88, 43, 64, 66, 12, 17, -37, -80, -34, 8, 0, 32, 12, -102, 102]

06-23 09:58:55.052  7999  5205 D BluetoothMapObexServer: onPut(): enter
06-23 09:58:55.052  7999  5205 D BluetoothMapObexServer: type = x-bt/MAP-NotificationRegistration, name = null
06-23 09:58:55.052  7999  5205 D BluetoothMapContentObserver: setNotificationRegistration() enter
06-23 09:58:55.053  7999  5205 D BluetoothMapContentObserver: setNotificationRegistration() send : 1 to MNS
06-23 09:58:55.090  7999  8130 D BluetoothMapService: ContentObserver Registration MASID: 0 Enable: 1
06-23 09:58:55.093  7999  5205 D BluetoothMapObexServer: onSetPath name is null backup: false create: false
06-23 09:58:55.103  7999  5205 D BluetoothMapObexServer: OnGet type is x-obex/folder-listing
06-23 09:58:55.116  7999  5205 D BluetoothMapObexServer: OnGet type is x-bt/MAP-msg-listing

06-23 09:58:55.334  7999  5205 V BluetoothMapObexServer: sendMessageListingRsp: has sms true, has email false, has IM false
06-23 09:58:55.334  7999  5205 D BluetoothMapContent: msgListingSize: folder = deleted
06-23 09:58:55.341  7999  5205 D BluetoothMapContent: phone type = 1 phone num = null phone alpha tag = null
06-23 09:58:55.341  7999  5205 D BluetoothMapContent: smsSelected msgType: 4
06-23 09:58:55.350  7999  5205 D BluetoothMapContent: mmsSelected msgType: 4
06-23 09:58:55.355  7999  9590 D BluetoothPbapService: getConnectionState: BC:30:7E:33:F3:55
06-23 09:58:55.356  5728  6150 D BluetoothMap: getConnectionState(BC:30:7E:33:F3:55)
06-23 09:58:55.357  7999  5205 D BluetoothMapContent: emailSelected msgType: 4
06-23 09:58:55.357  7999  5205 D BluetoothMapContent: imSelected msgType: 4
06-23 09:58:55.357  7999  5205 D BluetoothMapContent: msgListingSize: size = 0
06-23 09:58:55.357  7999  5205 D BluetoothMapContent: msgListingHasUnread: folder = deleted

```





