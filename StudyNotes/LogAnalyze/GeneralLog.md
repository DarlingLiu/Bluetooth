## Main log
bond state|connection state change|audio state changed:|A2dpStateMachine: Connection state|A2DP Playing state|setActiveDevice|btm_sec_dis|AvrcpVolumeManager: onAudioDevicesAdded|AvrcpVolumeManager: volumeDeviceSwitched

Bond, A2dp和Hfp连接状态：bond state|connection state change|A2dpStateMachine: Connection state|btm_acl_created

播放状态及ActiveDevice：A2DP Playing state|setActiveDevic

a2dp和hfp断开：btm_sec_dis|btm_acl_role_changed（主从切换），常见code: 8(connection timeout), 19(remote user terminated connection), 22(CONNECTION TERMINATED BY LOCAL HOST)

panic导致的蓝牙重启：AdapterState|Proxy object disconnected, 对应kernel log中wlbt fw panic

设置界面连接、配对、取消配对（对应类：CachedBluetoothDevice）：Command sent

ble设备连接不上，如status133：onClientConnectionState

查看手机蓝牙地址：get_local_address|AdapterProperties: Address|bt_btif : Remote device|BluetoothRemoteDevices: Remote Address

查看sco和a2dp编码：bt_wbs=|A2DP Codec Selectable|SelectSourceCodec: selected codec

avrcp：AvrcpVolumeManager: onAudioDevicesAdded|AvrcpVolumeManager: volumeDeviceSwitched

查找蓝牙进程中Error：pid[ ]+[0-9]+[ ]+E 

音乐播放暂停：MediaPlayerNative: start|AudioSink: start|MediaPlayerNative: pause|AudioSink: pause

蓝牙disable断开：BluetoothAdapterService: disable() called with mRunningProfiles.size() = 10

三星手机蓝牙地址：get_local_address|AdapterProperties: Address

建立sco： I bt_btm  : BTM_CreateSco: BTM_CreateSco succeeded

开始扫描和结束扫描：BluetoothAdapterService: startDiscovery|BluetoothAdapterService: cancelDiscovery （扫描ble设备需要打开定位，关闭定位会有：BluetoothUtils: Permission denial: Location is off）

BluetoothAdapter: isLeEnabled

startDiscovery|cancelDiscovery|isLeEnabled|BluetoothUtils: Permission denial

查看扫描到的设备（蓝牙设置界面）：type: 1(classic BR/EDR), 2(LE), 3(dual BR/EDR/LE), 0(Unknown)
04-20 16:19:14.461 13656 13656 I _V_DeviceListPreferenceFragment: device address is: 4E:8D:E6:B8:7A:8F device name is: 4E:8D:E6:B8:7A:8F type: 2 major class = 0x1f00
04-20 16:19:14.462 13656 13656 I _V_DeviceListPreferenceFragment: device address is: FC:AB:90:EC:CD:CC device name is: HUAWEI P30 Pro type: 1 major class = 0x200
04-20 16:19:14.465 13656 13656 I _V_DeviceListPreferenceFragment: device address is: D8:9C:67:53:C3:06 device name is: KD-75X8500F type: 3 major class = 0x400
04-20 16:19:14.468 13656 13656 I _V_DeviceListPreferenceFragment: device address is: E3:E2:48:5C:A3:B9 device name is: MAMBO type: 0 major class = 0x1f00

05-05 11:47:39.646117  3471  3498 D bt_btif : btif_in_fetch_bonded_ble_device Found a LE device: e2:94:16:97:87:07

05-05 11:47:39.646150  3471  3498 D bt_btif : Remote device:e2:94:16:97:87:07, no link key or ble key found

04-20 17:15:33.983 32664   562 D BluetoothGatt: connect() - device: C4:06:83:13:F5:E0, auto: false

04-20 17:15:34.425 30980 31041 D BtGatt.GattService: send ble connected broadcast
04-20 17:15:34.425 32664 32693 D BluetoothGatt: onClientConnectionState() - status=0 clientIf=6 device=C4:06:83:13:F5:E0

打电话切换接听方式：CallAudioRouteStateMachine

tx power: power_level
06-05 16:02:46.353 14336 14395 I bt_btif : btif_tx_power_log_vse_cback: Received parameters are: Connection_handle: 0x0002 piconet_clock: 0x00230110, rf_path: 0x01, power_level: 13
06-05 16:02:46.597 14336 14395 I bt_btif : btif_tx_power_log_vse_cback: Received parameters are: Connection_handle: 0x0002 piconet_clock: 0x00230414, rf_path: 0x01, power_level: 9
06-05 16:02:46.864 14336 14395 I bt_btif : btif_tx_power_log_vse_cback: Received parameters are: Connection_handle: 0x0002 piconet_clock: 0x00230770, rf_path: 0x01, power_level: 5
06-05 16:02:50.097 14336 14395 I bt_btif : btif_tx_power_log_vse_cback: Received parameters are: Connection_handle: 0x0002 piconet_clock: 0x00232FD4, rf_path: 0x01, power_level: 9
06-05 16:02:50.356 14336 14395 I bt_btif : btif_tx_power_log_vse_cback: Received parameters are: Connection_handle: 0x0002 piconet_clock: 0x00233310, rf_path: 0x01, power_level: 13
06-05 16:02:50.597 14336 14395 I bt_btif : btif_tx_power_log_vse_cback: Received parameters are: Connection_handle: 0x0002 piconet_clock: 0x00233618, rf_path: 0x02, power_level: 15


## HCI log
HCI_Read_Local_Supported_Commands中查看设备支持的HCI Command

HCI_Role_Change  role switch

HCI_Connection_Request  蓝牙设备主动发起连接，对应信息有设备地址

HCI_Create_Connection 手机主动发起连接

HCI_Connection_Complete 连接建立成功，对应信息有handle和设备地址

HCI_Synchronous_Connection_Complete  建立sco

HCI_LE_Extended_Advertising_Report：ble广播，详细信息中可以看到地址，信号强度，电量等信息

HCI_LE_Extended_Create_Connection：手机端发起ble设备连接操作

HCI_LE_Extended_Connection_Request：ble设备发起连接操作

HCI_Sniff_Subrating：ssr

HCI_Sniff_Mode：sniff mode
2020/6/15 15:34:56.373454 2,445 Event Vendor specific event 7 10 00:00:00.003435   → Vendor Specific Event: 0x 02 00 05 00 07 17
2020/6/15 15:34:56.374949 2,446 Event HCI_Mode_Change Success 0x0005 6 9 00:00:00.001495  →  Current_Mode: Sniff mode

2020/6/15 15:34:56.874244 2,451 Event Vendor specific event 7 10 00:00:00.453946   → Vendor Specific Event: 0x 02 00 05 00 06 18
2020/6/15 15:34:56.875079 2,452 Event HCI_Mode_Change Success 0x0005 6 9 00:00:00.000835  →  Current_Mode: Active mode



协议栈打log
```
#include <base/logging.h>
LOG(ERROR) << __func__ << ": unable to start btu message loop thread.";
```

打印调用信息
```
import android.os.Process;
Log.v(TAG, new Exception().getStackTrace()[0].getMethodName() + " PID = " + Process.myPid() + " TID = " + Process.myTid() + "UID = " + Binder.getCallingUid());
```