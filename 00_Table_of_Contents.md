Contents

Revision History ii

Contents iv

Tables xxiv

# 1Introduction 1

##  1.1 Overview

##  1

##  1.2 System Hang

##  2

# 2EFI Compliance Test 3

##  2.1 EFI Requirements Test

##  3

###  2.1.1 Required Elements

###  4

###  2.1.2 Platform-Specific Elements

###  6

# 3Services Boot Services 17

##  3.1 Event, Timer, and Task Priority Services Test

##  17

###  3.1.1 CreateEvent()

###  18

###  3.1.2 

### CloseEvent()

###  19

###  3.1.3 SignalEvent()

###  20

###  3.1.4 WaitForEvent()


###  20

###  3.1.5 CheckEvent()

###  22

###  3.1.6 SetTimer()

###  24

###  3.1.7 RaiseTPL()

###  26

###  3.1.8 

### RestoreTPL()

###  26

###  3.1.9 CreateEventEx()

###  27

##  3.2 

## Memory Allocation Services Test

##  30

###  3.2.1 

### AllocatePages()

###  31

###  3.2.2 FreePages()

###  74

###  3.2.3 GetMemoryMap()

###  76

###  3.2.4 AllocatePool()

###  83

###  3.2.5 FreePool()

###  85

##  3.3 

## Protocol Handler Services Test

##  85

###  3.3.1 InstallProtocolInterface()

###  87

###  3.3.2 UninstallProtocolInterface()

###  105

###  3.3.3 ReinstallProtocolInterface()

###  141

###  3.3.4 RegisterProtocolNotify() 167

###  3.3.5 LocateHandle()

###  178

###  3.3.6 HandleProtocol()

###  215

###  3.3.7 LocateDevicePath()

###  219

###  3.3.8 OpenProtocol()

###  223

###  3.3.9 CloseProtocol()

###  277

###  3.3.10 OpenProtocolInformation()

###  292

###  3.3.11 ConnectController() 317

###  3.3.12 DisconnectController()

###  365

###  3.3.13 ProtocolsPerHandle()

###  398

###  3.3.14 LocateHandleBuffer()

###  405

###  3.3.15 LocateProtocol()

###  427

###  3.3.16 InstallMultipleProtocolInterfaces()

###  433

###  3.3.17 UninstallMultipleProtocolInterfaces()

###  450

##  3.4 Image Services Test

##  495

###  3.4.1 

### LoadImage()

###  496

###  3.4.2 StartImage()

###  503

###  3.4.3 UnloadImage()

###  508

##  3.5 EFI_IMAGE_ENTRY_POINT

##  518

###  3.5.1 

### Exit() 

###  519

###  3.5.2 ExitBootServices()

###  526

##  3.6 Misc Boot Services Test

##  526

###  3.6.1 SetWatchdogTimer()

###  528

###  3.6.2 Stall() 535

###  3.6.3 CopyMem()

###  535

###  3.6.4 SetMem()

###  540

###  3.6.5 GetNextMonotonicCount()

###  542

###  3.6.6 InstallConfigurationTable()

###  546

###  3.6.7 CalculateCrc32()

###  556

# 4Services Runtime Services Test 559

##  4.1 Variable Services Test

##  559

###  4.1.1 GetVariable() 559

###  4.1.2 GetNextVariableName()

###  563

###  4.1.3 

### SetVariable()

###  564

###  4.1.4 QueryVariableInfo()

###  575

###  4.1.5 HardwareErrorRecord

###  577

##  4.2 

## Time Services Test

##  578

###  4.2.1 

### GetTime()

###  578

###  4.2.2 SetTime()

###  579

###  4.2.3 GetWakeupTime()

###  585

###  4.2.4 SetWakeupTime()

###  586

##  4.3 

## Virtual Memory Services Test

##  590

##  4.4 Misc Runtime Services Test

##  591

###  4.4.1 ResetSystem()

###  591

###  4.4.2 

### UpdateCapsule()

###  592

###  4.4.3 QueryCapsuleCapabilities()

###  593

###  4.4.4 

### GetNextHighMonotonicCount()

###  594

# 5Protocols EFI Loaded Image Test 595

##  5.1 EFI_LOADED_IMAGE Protocol Test

##  595

# 6Protocols Device Path Protocol Test 599

##  6.1 Device Path Node Conformance Test

##  599

##  6.2 Whole Device Path Conformance Test

##  607

##  6.3 Device Path Utilities Protocol Interface Function Test

##  609

###  6.3.1 CreatDeviceNode Functionality

###  609

###  6.3.2 

### AppendDeviceNode Functionality

###  609

###  6.3.3 

### GetDevicePathSize Functionality

###  611

###  6.3.4 

### DuplicateDevicePath Functionality

###  611

###  6.3.5 DuplicateDevicePath Conformance

###  611

###  6.3.6 

### AppendDevicePath Functionality

###  612

###  6.3.7 AppendDevicePathInstance Functionality

###  612

###  6.3.8 

### GetNextDevicePathInstance Functionality

###  613

###  6.3.9 

### IsDevicePathMultiInstance Functionality

###  613

##  6.4 Device Path Utilities Protocol Interface Conformance Test

##  614

###  6.4.1 CreatDeviceNode Conformance

###  614

###  6.4.2 AppendDeviceNode Conformance

###  614

###  6.4.3 

### AppendDevicePath Conformance

###  615

###  6.4.4 

### AppendDevicePathInstance Conformance

###  615

###  6.4.5 

### GetNextDevicePathInstance Conformance

###  616

##  6.5 

## Device Path To Text Protocol Interface Function Test

##  616

###  6.5.1 ConvertDeviceNodeToText Functionality

###  616

###  6.5.2 

### ConvertDevicePathToText Functionality

###  617

##  6.6 Device Path To Text Protocol Interface Conformance Test

##  618

###  6.6.1 ConvertDeviceNodeToText Conformance

###  618

###  6.6.2 

### ConvertDevicePathToText Conformance

###  618

##  6.7 Device Path To Text Protocol Interface Coverage Test

##  619

###  6.7.1 ConvertDeviceNodeToText Coverage

###  619

###  6.7.2 

### ConvertDevicePathToText Coverage

###  630

##  6.8 

## Device Path From Text Protocol Interface Function Test

##  631

###  6.8.1 ConvertTextToDeviceNode Functionality

###  631

###  6.8.2 

### ConvertTextToDevicePath Functionality

###  632

##  6.9 Device Path From Text Protocol Interface Conformance Test

##  632

###  6.9.1 ConvertTextToDeviceNode Conformance

###  632

###  6.9.2 

### ConvertTextToDevicePath Conformance

###  633

##  6.10 Device Path From Text Protocol Interface Coverage Test

##  634

###  6.10.1 ConvertTextToDeviceNode Coverage

###  634

###  6.10.2 ConvertTextToDevicePath Coverage

###  647

# 7Protocols EFI Driver Model Test 649

##  7.1 EFI_DRIVER_BINDING_PROTOCOL Test

##  649

##  7.2 EFI_PLATFORM_DRIVER_OVERRIDE_PROTOCOL Test

##  649

###  7.2.1 GetDriver()

###  649

###  7.2.2 GetDriverPath()

###  650

###  7.2.3 DriverLoaded()

###  651

##  7.3 

## EFI_BUS_SPECIFIC_DRIVER_OVERRIDE_PROTOCOL Test

##  652

###  7.3.1 GetDriver()

###  652

##  7.4 

## EFI_DRIVER_CONFIGURATION_PROTOCOL Test

##  652

###  7.4.1 SetOptions()

###  653

###  7.4.2 OptionsValid()

###  654

###  7.4.3 

### ForceDefaults()

###  654

##  7.5 

## EFI_DRIVER_DIAGNOSTICS_PROTOCOL Test

##  655

###  7.5.1 RunDiagnostic()

###  655

##  7.6 

## EFI_DRIVER_DIAGNOSTICS2_PROTOCOL Test

##  656

###  7.6.1 RunDiagnostic()

###  656

##  7.7 

## EFI_COMPONENT_NAME_PROTOCOL Test

##  658

###  7.7.1 GetDriverName()

###  658

###  7.7.2 GetControllerName()

###  659

##  7.8 

## EFI_COMPONENT_NAME2_PROTOCOL Test

##  662

###  7.8.1 GetDriverName()

###  662

###  7.8.2 

### GetControllerName()

###  663

##  7.9 

## EFI_PLATFORM_TO_DRIVER_CONFIGURATION_PROTOCOL

##  664

###  7.9.1 Query()

###  665

###  7.9.2 

### Response()

###  665

###  7.9.3 

### DMTF SM CLP ParameterTypeGuid

###  666

##  7.10 EFI_DRIVER_SUPPORTED_EFI_VERSION_PROTOCOL Test

##  667

##  7.11 


## EFI_ADAPTER_INFORMATION_PROTOCOL Test

##  667

###  7.11.1 GetInformation() 667

###  7.11.2 SetInformation() 669

###  7.11.3 GetSupportedTypes() 670

# 8Protocols Console Support Test 673

##  8.1 EFI_SIMPLE\_ TEXT_INPUT_PROTOCOL Test 673

###  8.1.1 Reset() 673

###  8.1.2 ReadKeyStroke() 673

##  8.2 EFI_SIMPLE_TEXT_OUTPUT_PROTOCOL Test 674

###  8.2.1 Reset() 674

###  8.2.2 OutputString() 675

###  8.2.3 TestString() 676

###  8.2.4 QueryMode() 676

###  8.2.5 SetMode() 678

###  8.2.6 SetAttribute() 678

###  8.2.7 ClearScreen() 679

###  8.2.8 SetCursorPosition() 680

###  8.2.9 EnableCursor() 681

##  8.3 EFI_SIMPLE_POINTER_PROTOCOL_PROTOCOL Test 682

###  8.3.1 Reset() 682

###  8.3.2 GetState() 683

##  8.4 EFI_SERIAL_IO_PROTOCOL Test 684

###  8.4.1 Reset() 684

###  8.4.2 SetAttributes() 685

###  8.4.3 SetControl() 687

###  8.4.4 GetControl() 688

###  8.4.5 Write() 688

###  8.4.6 Read() 689

##  8.5 EFI_GRAPHICS_OUTPUT_PROTOCOL Test 690

###  8.5.1 QueryMode() 690

###  8.5.2 SetMode() 693

###  8.5.3 Blt() 695

##  8.6 EFI_SIMPLE\_ TEXT_INPUT_EX_PROTOCOL Test 734

###  8.6.1 Reset() 734

###  8.6.2 ReadKeyStrokeEx () 735

###  8.6.3 SetState () 736

###  8.6.4 RegisterKeyNotify () 736

###  8.6.5 UnregisterKeyNotify () 738

##  8.7 EFI_ABSOLUTE_POINTER_PROTOCOL Test 739

###  8.7.1 Reset() 739

###  8.7.2 GetState() 740

# 9Protocols Bootable Image Support Test 743

##  9.1 EFI_LOAD_FILE_PROTOCOL Test

##  743

##  9.2 EFI_SIMPLE_FILE_SYSTEM_PROTOCOL Test

##  743

###  9.2.1 OpenVolume()

###  743

##  9.3 EFI_FILE_PROTOCOL Test

##  746

###  9.3.1 Open()

###  746

###  9.3.2 Close()

###  755

###  9.3.3 

### Delete()

###  756

###  9.3.4 Read()

###  759

###  9.3.5 Write()

###  762

###  9.3.6 Flush()

###  765

###  9.3.7 SetPosition()

###  766

###  9.3.8 GetPosition()

###  768

###  9.3.9 GetInfo()

###  769

###  9.3.10 SetInfo()

###  774

###  9.3.11 OpenEx() 780

###  9.3.12 ReadEx 794

###  9.3.13 WriteEX 797

###  9.3.14 FlushEx 800

###  9.3.15 Read-Only File System check points 802

##  9.4 EFI_DISK_IO_PROTOCOL Test

##  805

###  9.4.1 ReadDisk()

###  806

###  9.4.2 

### WriteDisk() 809

##  9.5 

## EFI_BLOCK_IO_PROTOCOL Test

##  812

###  9.5.1 Reset()

###  812

###  9.5.2 ReadBlocks()

###  813

###  9.5.3 WriteBlocks()

###  815

###  9.5.4 

### FlushBlocks()

###  819

###  9.5.5 Media Info Check 819

##  9.6 EFI_UNICODE_COLLATION_PROTOCOL Test

##  820

###  9.6.1 StriColl()

###  820

###  9.6.2 

### MetaiMatch()


###  820

###  9.6.3 StrLwr()

###  820

###  9.6.4 StrUpr()

###  821

###  9.6.5 

### FatToStr()

###  821

###  9.6.6 

### StrToFat()

###  822

##  9.7 

## EFI_UNICODE_COLLATION2_PROTOCOL Test

##  822

###  9.7.1 StriColl()


###  823

###  9.7.2 MetaiMatch()

###  823

###  9.7.3 

### StrLwr()

###  823

###  9.7.4 StrUpr()

###  824

###  9.7.5 FatToStr()

###  824

###  9.7.6 StrToFat()

###  825

##  9.8 EFI_ATA_PASS_THRU_PROTOCOL Test

##  825

###  9.8.1 GetNextPort()

###  825

###  9.8.2 BuildDevicePath() 826

###  9.8.3 

### GetDevice() 827

###  9.8.4 

### ResetPort() 

###  827

###  9.8.5 

### ResetDevice()

###  828

###  9.8.6 

### GetNextDevice() 828

###  9.8.7 PassThru() 829

###  9.8.8 Mode Conformance




###  833

##  9.9 EFI_BLOCK_IO2_PROTOCOL Test

##  833

###  9.9.1 ReadBlocksEx()

###  834

###  9.9.2 WriteBlocksEx()

###  836

###  9.9.3 FlashBlocksEx()

###  838

###  9.9.4 Media Info Check 839

##  9.10 EFI_STORAGE_SECURITY_COMMAND_PROTOCOL Test

##  839

###  9.10.1 ReceiveData()

###  840

###  9.10.2 

### SendData()

###  840

##  9.11 EFI_DISK_IO2_PROTOCOL Test 841

###  9.11.1 Cancel() 841

###  9.11.2 ReadDiskEx() 841

###  9.11.3 

### WriteDiskEx() 844

###  9.11.4 FlushDiskEx() 846

###  9.11.5 EFI_NVM_EXPRESS_PASS_THRU_PROTOCOL Test 848

###  9.11.6 PassThru() 848

###  9.11.7 GetNextNamespace() 851

###  9.11.8 BuildDevicePath() 851

###  9.11.9 GetNamespace() 852

##  9.12 EFI_NVM_EXPRESS_PASS_THRU_PROTOCOL Test 854

###  9.12.1 PassThru() 854

###  9.12.2 GetNextNamespace() 855

###  9.12.3 BuildDevicePath() 855

###  9.12.4 GetNamespace() 857

##  9.13 EFI_ERASE_BLOCK_PROTOCOL Test 858

###  9.13.1 EraseBlocks() 858

##  9.14 EFI_SD_MMC_PASS_THRU_PROTOCOL Test 860

###  9.14.1 PassThru() 860

###  9.14.2 GetNextSlot() 861

###  9.14.3 BuildDevicePath() 861

###  9.14.4 GetSlotNumber() 862

###  9.14.5 ResetDevice() 862

##  9.15 EFI_RAM_DISK_PROTOCOL Test 863

###  9.15.1 Register() 863

###  9.15.2 Unregister() 864

# 10Protocols PCI Bus Support Test 865

##  10.1 EFI_PCI_ROOT_BRIDGE_IO_PROTOCOL Test

##  865

###  10.1.1 PollMem()

###  865

###  10.1.2 PollIo()

###  867

###  10.1.3 Mem.Read()

###  869

###  10.1.4 

### Mem.Write()

###  871

###  10.1.5 Io.Read()

###  873

###  10.1.6 Io.Write()

###  875

###  10.1.7 Pci.Read()

###  878

###  10.1.8 Pci.Write()

###  880

###  10.1.9 CopyMem()

###  882

###  10.1.10 Map()

###  884

###  10.1.11 Unmap()

###  889

###  10.1.12 AllocateBuffer()

###  891

###  10.1.13 FreeBuffer()

###  892

###  10.1.14 

### Flush()

###  892

###  10.1.15 GetAttributes()

###  893

###  10.1.16 SetAttributes()

###  894

###  10.1.17 

### Configuration()

###  897

##  10.2 EFI_PCI_IO_PROTOCOL Test

##  897

###  10.2.1 PollMem()

###  897

###  10.2.2 PollIo()

###  900

###  10.2.3 Mem.Read()

###  902

###  10.2.4 Mem.Write()

###  905

###  10.2.5 Io.Read()

###  908

###  10.2.6 Io.Write()

###  911

###  10.2.7 Pci.Read()

###  914

###  10.2.8 Pci.Write()

###  917

###  10.2.9 CopyMem()

###  919

###  10.2.10 Map()

###  923

###  10.2.11 Unmap()

###  927

###  10.2.12 AllocateBuffer()

###  928

###  10.2.13 FreeBuffer()

###  929

###  10.2.14 

### Flush()

###  930

###  10.2.15 GetLocation()

###  930

###  10.2.16 Attributes()

###  931

###  10.2.17 GetBarAttributes()

###  935

###  10.2.18 SetBarAttributes()

###  937

# 11Protocols USB Support Test 939

##  11.1 EFI_USB2_HC_PROTOCOL Test

##  939

###  11.1.1 GetCapability()

###  939

###  11.1.2 Reset()

###  940

###  11.1.3 

### GetState()

###  941

###  11.1.4 SetState()

###  942

###  11.1.5 ControlTransfer()

###  944

###  11.1.6 BulkTransfer()

###  946

###  11.1.7 AsyncInterruptTransfer()

###  948

###  11.1.8 SyncInterruptTransfer()

###  949

###  11.1.9 IsochronousTransfer()

###  950

###  11.1.10 

### AsyncIsochronousTransfer()

###  951

###  11.1.11 

### GetRootHubPortStatus()

###  952

###  11.1.12 

### SetRootHubPortFeature()

###  952

###  11.1.13 

### ClearRootHubPortFeature()

###  953

##  11.2 

## EFI_USB_IO_PROTOCOL Test

##  954

###  11.2.1 UsbControlTransfer()

###  954

###  11.2.2 UsbBulkTransfer()

###  955

###  11.2.3 UsbAsyncInterruptTransfer()

###  956

###  11.2.4 UsbSyncInterruptTransfer()

###  958

###  11.2.5 UsbIsochronousTransfer()

###  960

###  11.2.6 UsbAsyncIsochronousTransfer()

###  961

###  11.2.7 

### UsbGetDeviceDescriptor()

###  962

###  11.2.8 

### UsbGetConfigDescriptor()

###  963

###  11.2.9 

### UsbGetInterfaceDescriptor()

###  963

###  11.2.10 UsbGetEndpointDescriptor()

###  963

###  11.2.11 

### UsbPortReset()

###  964

# 12Protocols SCSI Bus Support Test 965

##  12.1 EFI_SCSI_IO_PROTOCOL Function Test

##  965

###  12.1.1 GetDeviceType() Function

###  965

###  12.1.2 

### GetDeviceLocation() Function


###  965

###  12.1.3 ResetBus() Function

###  965

###  12.1.4 ResetDevice() Function

###  966

###  12.1.5 

### ExecuteScsiCommand () Function

###  966

##  12.2 

## EFI_SCSI_IO_PROTOCOL Conformance Test

##  967

###  12.2.1 GetDeviceType() Conformance

###  967

###  12.2.2 GetDeviceLocation() Conformance

###  967

###  12.2.3 ExecuteScsiCommand () Conformance

###  968

##  12.3 EFI_EXT_SCSI_PASS_PROTOCOL Function Test 

##  969

###  12.3.1 GetNextTargetLun() Function

###  969

###  12.3.2 

### BuildDevicePath() Function

###  969

###  12.3.3 

### GetTargetLun() Function

###  969

###  12.3.4 ResetChannel() Function

###  970

###  12.3.5 

### ResetTargetLun() Function

###  970

###  12.3.6 

### GetNextTarget () Function

###  970

###  12.3.7 PassThru () Function

###  970

##  12.4 

## EFI_EXT_SCSI_PASS_PROTOCOL Conformance Test 

##  971

###  12.4.1 GetNextTargetLun() Conformance

###  971

###  12.4.2 BuildDevicePath() Conformance

###  972

###  12.4.3 GetTargetLun() Conformance

###  972

###  12.4.4 ResetTargetLun() Conformance

###  973

###  12.4.5 GetNextTarget () Conformance

###  973

###  12.4.6 PassThru() Conformance

###  974

# 13Protocols iSCSI Boot Test

#  977

##  13.1 EFI_ISCSI_INITIATOR_NAME_PROTOCOL Function Test

##  977

###  13.1.1 Get() Function

###  977

###  13.1.2 

### Set() Function

###  977

##  13.2 EFI_ISCSI_INITIATOR_NAME_PROTOCOL Conformance Test

##  978

###  13.2.1 Get() Conformance

###  978

###  13.2.2 Set() Conformance

###  978

# 14Network Protocols SNP, PXE and BISTest 981

##  14.1 EFI_SIMPLE_NETWORK_PROTOCOL Test

##  981

###  14.1.1 Start()

###  981

###  14.1.2 Stop()

###  981

###  14.1.3 Initialize()

###  982

###  14.1.4 Reset()

###  982

###  14.1.5 

### Shutdown()

###  983

###  14.1.6 ReceiveFilters()

###  983

###  14.1.7 StationAddress()

###  986

###  14.1.8 Statistics()

###  987

###  14.1.9 MCastIPtoMAC()

###  988

###  14.1.10 NvData()

###  988

###  14.1.11 GetStatus()

###  990

###  14.1.12 Transmit()

###  991

###  14.1.13 Receive()

###  993

##  14.2 EFI_PXE_BASE_CODE_PROTOCOL Test

##  994

###  14.2.1 Start()

###  994

###  14.2.2 Stop()

###  995

###  14.2.3 

### Dhcp()

###  995

###  14.2.4 Discover()

###  995

###  14.2.5 Mtftp()

###  995

###  14.2.6 UdpWrite()

###  995

###  14.2.7 UdpRead()

###  996

###  14.2.8 SetIpFilter()

###  996

###  14.2.9 

### Arp() 996

###  14.2.10 SetParameters()

###  997

###  14.2.11 SetStationIp()

###  997

###  14.2.12 

### SetPackets()

###  998

##  14.3 

## EFI_PXE_BASE_CODE_CALLBACK_PROTOCOL Test

##  998

##  14.4 EFI_BIS_PROTOCOL Test

##  998

# 15Protocols Compression Test 999

##  15.1 EFI_DECOMPRESS_PROTOCOL Test

##  999

###  15.1.1 GetInfo()

###  999

###  15.1.2 Decompress() 1000

# 16Protocols Debugger Support Test 1003

##  16.1 EFI_DEBUG_SUPPORT_PROTOCOL Test

##  1003

###  16.1.1 GetMaximumProcessorIndex()

###  1003

###  16.1.2 RegisterPeriodicCallback()

###  1003

###  16.1.3 RegisterExceptionCallback()

###  1005

###  16.1.4 

### InvalidateInstructionCache()

###  1006

###  16.1.5 

### Isa

###  1006

##  16.2 EFI_DEBUGPORT_PROTOCOL Test

##  1006

###  16.2.1 Reset()

###  1006

###  16.2.2 

### Write()

###  1007

###  16.2.3 Read()

###  1007

###  16.2.4 Poll()

###  1007

# 17Protocols ACPI Test 1009

##  17.1 EFI_ACPI_TABLE_PROTOCOL Test

##  1009

###  17.1.1 InstallAcpiTable ()

###  1009

###  17.1.2 UninstallAcpiTable ()

###  1010

# 18Network Protocols Managed Network 1011

##  18.1 EFI_MANAGED_NETWORK_PROTOCOL Test

##  1011

###  18.1.1 GetModeData()

###  1011

###  18.1.2 Configure()

###  1013

###  18.1.3 McastlpToMac()

###  1015

###  18.1.4 Groups()

###  1018

###  18.1.5 Transmit()

###  1022

###  18.1.6 

### Receive()

###  1027

###  18.1.7 Cancel()

###  1030

###  18.1.8 Poll()

###  1032

###  18.1.9 CreateChild()

###  1033

###  18.1.10 DestroyChild()

###  1034

# 19EFI Byte Code Virtual Machine Test 1035

##  19.1 EFI_EBC_PROTOCOL Test

##  1035

###  19.1.1 CreateThunk()

###  1035

###  19.1.2 UnloadIImage()

###  1036

###  19.1.3 

### RegisterICacheFlush()

###  1036

###  19.1.4 GetVersion()

###  1037

# 20Network Protocols ARP and DHCP 1039

##  20.1 EFI_ARP_PROTOCOL Test

##  1039

###  20.1.1 Add()


###  1039

###  20.1.2 Cancel()

###  1054

###  20.1.3 Configure()

###  1061

###  20.1.4 Delete() 1071

###  20.1.5 Find()

###  1077

###  20.1.6 Flush()

###  1092

###  20.1.7 

### Request()

###  1094

###  20.1.8 CreateChild()

###  1108

###  20.1.9 DestroyChild()

###  1108

###  20.1.10 RFC Related

###  1109

##  20.2 EFI_DHCP4_PROTOCOL Test

##  1110

###  20.2.1 GetModeData()


###  1111

###  20.2.2 Configure()

###  1114

###  20.2.3 

### Start()

###  1120

###  20.2.4 RenewRebind()

###  1129

###  20.2.5 Release()

###  1140

###  20.2.6 Stop()

###  1143

###  20.2.7 

### Build()

###  1145

###  20.2.8 

### Transmit**Receive()**

###  1148

###  20.2.9 Parse()

###  1150

###  20.2.10 

### CreateChild()


###  1153

###  20.2.11 DestroyChild()

###  1154

##  20.3 EFI_DHCP6_PROTOCOL Test

##  1155

###  20.3.1 CreateChild()

###  1155

###  20.3.2 DestroyChild ()

###  1156

###  20.3.3 GetModeData()

###  1156

###  20.3.4 

### Configure() 1159

###  20.3.5 Start()

###  1162

###  20.3.6 InfoRequest()

###  1163

###  20.3.7 RenewRebind()

###  1166

###  20.3.8 Decline()

###  1168

###  20.3.9 Release()

###  1172

###  20.3.10 Stop()

###  1175

###  20.3.11 Parse()

###  1177

# 21Network Protocols TCP, IP and Configuration 1179

##  21.1 EFI_TCP4_PROTOCOL Test

##  1179

###  21.1.1 GetModeData()

###  1179

###  21.1.2 Configure()

###  1192

###  21.1.3 Connect()

###  1196

###  21.1.4 Accept()

###  1199

###  21.1.5 

### Transmit()

###  1204

###  21.1.6 Receive()

###  1212

###  21.1.7 Close()

###  1223

###  21.1.8 

### CnntClosing

###  1226

###  21.1.9 CnntOpening

###  1236

###  21.1.10 CongestionCtrl

###  1246

###  21.1.11 NagleSWSA

###  1253

###  21.1.12 UrgHandling

###  1261

###  21.1.13 

### RstHandling

###  1270

###  21.1.14 WinFlowCtrl

###  1292

###  21.1.15 Options

###  1304

###  21.1.16 

### Others

###  1321

###  21.1.17 KeepAliveTimer

###  1328

###  21.1.18 RetransmissiomTimer

###  1329

###  21.1.19 

### HrdFormatACK

###  1330

###  21.1.20 

### HrdFormatCheckSum

###  1331

###  21.1.21 PersistTimer

###  1331

##  21.2 

## EFI_IP4_PROTOCOL Test

##  1332

###  21.2.1 GetModeData()

###  1333

###  21.2.2 

### Configure()

###  1338

###  21.2.3 Groups()

###  1343

###  21.2.4 

### Routes()

###  1349

###  21.2.5 Transmit()

###  1360

###  21.2.6 Receive()

###  1377

###  21.2.7 Cancel()

###  1383

###  21.2.8 

### Poll()

###  1386

###  21.2.9 CreateChild()

###  1386

###  21.2.10 DestroyChild()

###  1387

##  21.3 EFI_IP4_CONFIG_PROTOCOL Test

##  1388

###  21.3.1 Start()

###  1389

###  21.3.2 Stop()

###  1391

###  21.3.3 GetData()

###  1393

##  21.4 EFI_TCP6_PROTOCOL Test

##  1397

###  21.4.1 CreateChild()/DestroyChild()

###  1398

###  21.4.2 GetModeData()

###  1399

###  21.4.3 Configure()

###  1401

###  21.4.4 Connect()

###  1403

###  21.4.5 Accept()

###  1406

###  21.4.6 Transmit()

###  1408

###  21.4.7 Receive() 1411

###  21.4.8 Close()

###  1414

##  21.5 

## EFI_IP6_PROTOCOL Test

##  1416

###  21.5.1 CreateChild()

###  1417

###  21.5.2 DestoryChild()

###  1418

###  21.5.3 GetModeData()

###  1418

###  21.5.4 Configure()

###  1419

###  21.5.5 Groups()

###  1422

###  21.5.6 Routes()

###  1424

###  21.5.7 Neighbors()

###  1427

###  21.5.8 

### Transmit()

###  1432

###  21.5.9 Receive()

###  1437

###  21.5.10 Cancel()

###  1440

###  21.5.11 

### Poll()

###  1441

##  21.6 EFI_IP6CONFIG_PROTOCOL Test

##  1442

###  21.6.1 SetData()

###  1443

###  21.6.2 GetData()

###  1447

###  21.6.3 RegisterDataNotify()

###  1449

###  21.6.4 UnregisterDataNotify()

###  1451

##  21.7 EFI_IPSEC_CONFIG_PROTOCOL Test

##  1452

###  21.7.1 SetData()

###  1453

###  21.7.2 GetData()

###  1457

###  21.7.3 GetNextSelector ()

###  1461

###  21.7.4 RegisterDataNotify ()

###  1464

###  21.7.5 UnregisterDataNotify ()

###  1465

##  21.8 EFI_IPSEC2_PROTOCOL Test

##  1465

###  21.8.1 ProcessExt()

###  1466

# 22Network Protocols UDP and MTFTP 1473

##  22.1 EFI_UDP4_PROTOCOL Test

##  1473

###  22.1.1 GetModeData()


###  1473

###  22.1.2 Configure()

###  1478

###  22.1.3 Groups()

###  1490

###  22.1.4 Routes()

###  1495

###  22.1.5 

### Transmit()

###  1500

###  22.1.6 

### Receive()

###  1509

###  22.1.7 

### Cancel()

###  1512

###  22.1.8 Poll()

###  1514

###  22.1.9 


### CreateChild()

###  1514

###  22.1.10 

### DestroyChild() 1515

##  22.2 

## EFI_MTFTP4_PROTOCOL Test

##  1515

###  22.2.1 CreateChild()

###  1516

###  22.2.2 DestroyChild()

###  1518

###  22.2.3 

### GetModeData()

###  1520

###  22.2.4 Configure()

###  1521

###  22.2.5 GetInfo()

###  1525

###  22.2.6 

### ParseOptions()

###  1536

###  22.2.7 

### ReadFile()

###  1541

###  22.2.8 

### WriteFile()

###  1604

###  22.2.9 

### ReadDirectory()

###  1620

###  22.2.10 

### Poll()

###  1626

##  22.3 EFI_UDP6_PROTOCOL Test

##  1626

###  22.3.1 CreateChild()

###  1627

###  22.3.2 DestoryChild()

###  1627

###  22.3.3 GetModeData()

###  1628

###  22.3.4 Configure()

###  1629

###  22.3.5 Groups()

###  1631

###  22.3.6 Transmit()

###  1633

###  22.3.7 Receive()

###  1636

###  22.3.8 Cancel()

###  1638

##  22.4 EFI_MTFTP6_PROTOCOL Test

##  1639

###  22.4.1 CreateChild()

###  1639

###  22.4.2 DestroyChild ()

###  1640

###  22.4.3 

### GetModeData()

###  1640

###  22.4.4 Configure()

###  1641

###  22.4.5 GetInfo()

###  1643

###  22.4.6 

### ParseOptions()

###  1646

###  22.4.7 ReadFile()

###  1647

###  22.4.8 WriteFile()

###  1653

###  22.4.9 ReadDirectory()

###  1657

###  22.4.10 

### Poll()

###  1662

# 23Network Protocols VLAN and EAP 1663

##  23.1 EFI_VLAN_CONFIG_PROTOCOL Test

##  1663

###  23.1.1 Set()

###  1663

###  23.1.2 

### Find()

###  1664

###  23.1.3 

### Remove()

###  1665

# 24EFI Tape IO to Test 1667

##  24.1 EFI_TAPE_IO_PROTOCOL Test

##  1667

###  24.1.1 TapeRead()

###  1667

###  24.1.2 TapeWrite()

###  1668

###  24.1.3 

### TapeRewind()

###  1669

###  24.1.4 


### TapeSpace()

###  1670

###  24.1.5 


### TapeWriteFM()

###  1671

###  24.1.6 

### TapeReset()

###  1672

# 25Protocols Security Test 1673

##  25.1 HASH Protocol Test

##  1673

###  25.1.1 GetHashSize()

###  1673

###  25.1.2 Hash() 1674

##  25.2 

## AUTHENTICATION_INFO Protocol Test

##  1675

###  25.2.1 Get()

###  1676

###  25.2.2 


### Set()

###  1676

##  25.3 EFI_HASH2_PROTOCOL Test 1677

###  25.3.1 GetHashSize () 1677

###  25.3.2 Hash() 1678

###  25.3.3 HashInit() 1678

###  25.3.4 HashUpdate() 1679

###  25.3.5 HashFinal() 1679

##  25.4 EFI_PKCS7_VERIFY_PROTOCOL Test 1681

###  25.4.1 VerifyBuffer() 1681

# 26Protocols EFI Firmware Management Test Case 1685

##  26.1 EFI_FIRMWARE_MANAGEMENT_PROTOCOL

##  1685

###  26.1.1 

### GetImageInfo()

###  1685

###  26.1.2 

### GetImage()

###  1686

###  26.1.3 SetImage()

###  1686

###  26.1.4 

### CheckImage()

###  1687

###  26.1.5 GetPackageInfo()

###  1687

###  26.1.6 

### SetPackageInfo()

###  1688

# 27Protocols HII Test 1689

##  27.1 EFI_HII_FONT_PROTOCOL Test

##  1689

###  27.1.1 StringToImage()

###  1689

###  27.1.2 StringIdToImage()

###  1695

###  27.1.3 GetGlyph()

###  1696

###  27.1.4 GetFontInfo()

###  1697

##  27.2 

## EFI_HII_STRING_PROTOCOL Test

##  1697

###  27.2.1 NewString()

###  1698

###  27.2.2 GetString()

###  1699

###  27.2.3 SetString()

###  1701

###  27.2.4 GetLanguages()

###  1703

###  27.2.5 GetSecondaryLanguages()

###  1704

##  27.3 

## EFI_HII_IMAGE_PROTOCOL Test

##  1705

###  27.3.1 NewImage()

###  1706

###  27.3.2 GetImage()

###  1707

###  27.3.3 SetImage()

###  1709

###  27.3.4 DrawImage()

###  1710

###  27.3.5 DrawImageId()

###  1712

##  27.4 EFI_HII_DATABASE_PROTOCOL Test

##  1713

###  27.4.1 NewPackageList ()

###  1714

###  27.4.2 RemovePackageList ()

###  1715

###  27.4.3 UpdatePackageList ()

###  1716

###  27.4.4 ListPackageLists()

###  1717

###  27.4.5 ExportPackageLists ()

###  1719

###  27.4.6 RegisterPackageNotify()

###  1721

###  27.4.7 UnregisterPackageNotify()

###  1722

###  27.4.8 FindKeyboardLayouts()

###  1723

###  27.4.9 GetKeyboardLayout()

###  1724

###  27.4.10 SetKeyboardLayout()

###  1725

###  27.4.11 GetPackageListHandle()

###  1726

##  27.5 EFI_HII_CONFIG_ROUTING_PROTOCOL Test

##  1727

###  27.5.1 ExtractConfig()

###  1728

###  27.5.2 ExportConfig()

###  1729

###  27.5.3 RouteConfig()

###  1730

###  27.5.4 BlockToConfig()

###  1731

###  27.5.5 

### ConfigToBlock ()

###  1732

###  27.5.6 

### GetAltCfg ()

###  1733

##  27.6 EFI_HII_CONFIG_ACCESS_PROTOCOL Test

##  1734

###  27.6.1 ExtractConfig()

###  1735

###  27.6.2 

### RouteConfig()

###  1737

##  27.7 EFI_CONFIG_KEYWORD_HANDLER_PROTOCOL Test 1737

###  27.7.1 SetData() 1738

###  27.7.2 GetData() 1741

##  27.8 EFI_HII_FONT_EX_PROTOCOL Test 1743

###  27.8.1 StringToImageEx() 1744

###  27.8.2 StringIdToImageEx() 1750

###  27.8.3 GetGlyphEx() 1752

###  27.8.4 GetFontInfoEx() 1752

###  27.8.5 GetGlyphInfo() 1753

##  27.9 EFI_HII_IMAGE_EX_PROTOCOL Test 1754

###  27.9.1 NewImageEx() 1754

###  27.9.2 GetImageEx() 1755

###  27.9.3 SetImageEx() 1756

###  27.9.4 DrawImageEx() 1757

###  27.9.5 DrawImageIdEx() 1758

###  27.9.6 GetImageInfo() 1760

# 28Random Number Generator Protocols 1761

##  28.1 EFI_RNG_PROTOCOL Test

##  1761

###  28.1.1 GetInfo () 1761

###  28.1.2 GetRNG() 1762

# 29Timestamp Protocols 1765

##  29.1 EFI_TIMESTAMP_PROTOCOL Test

##  1765

###  29.1.1 GetTimestamp()

###  1765

###  29.1.2 

### GetProperties()

###  1765

# 30Protocols String Services Test 1767

##  30.1 EFI_REGULAR_EXPRESSION_PROTOCOL Test 1767

###  30.1.1 MatchString() 1767

###  30.1.2 GetInfo() 1768

Appendix A  
Format of Test Profiles 1769

A.1EFI Requirements Test Profile

1769

A.2EFI_PCI_ROOT_BRIDGE_IO_PROTOCOL Test Profile

1769

A.3

EFI_PCI_IO_PROTOCOL Test Profile

1772

A.4EFI_DEVICE_IO_PROTOCOL Test Profile

1776

Appendix B  
Deprecated Protocols 1779

B.1Deprecated Protocols

1781

B.2

EFI_UGA_DRAW_PROTOCOL Test

1781

B.3EFI_SCSI_PASS_THRU_PROTOCOL Test

1787
