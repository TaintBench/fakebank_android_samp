# PROFILE
# Installation:
![ICON](icon.png)
# General Information:
- **fileName**: fakebank_android_samp.apk
- **packageName**: com.example.smsmanager
- **targetSdk**: 10
- **minSdk**: 7
- **maxSdk**: 15
- **mainActivity**: com.example.bankmanager.BankSplashActivity
# Behavior Information:
## Activities:
- When executed, the malware asks the user to enter in their banking account details.
- Collected details are sent to a remote URL  http://kkk.kakatt.net:3369/send_bank.php 
## BroadcastReceivers: 
- BootCompleteBroadcastReceiver steals SIM card serial number and sends them to a remote URL http://www.shm2580.com/post_simno.asp 
- smsReceiver monitors incoming SMS messages and sends them to a remote URL http://kkk.kakatt.net:3369/send_product.php 
## Services: 
- SmsSystemManageService keeps the screen on. 
- InstallService allows packages to be installed or deleted.
# Detail Information:
## Activities: 7
	.MessageActivity
	com.example.bankmanager.BankNumActivity
	com.example.bankmanager.BankScardActivity
	com.example.bankmanager.BankEndActivity
	com.example.bankmanager.BankActivity
	com.example.bankmanager.BankPreActivity
	com.example.bankmanager.BankSplashActivity
## Services: 2
	com.example.service.InstallService
	.SmsSystemManageService
## Receivers: 3
	.AlarmReceiver
	.BootCompleteBroadcastReceiver
	.smsReceiver
## Permissions: 15
	android.permission.RECEIVE_SMS
	android.permission.SEND_SMS
	android.permission.WRITE_SMS
	android.permission.READ_CONTACTS
	android.permission.READ_SMS
	android.permission.MOUNT_UNMOUNT_FILESYSTEMS
	android.permission.INSTALL_PACKAGES
	android.permission.RECEIVE_BOOT_COMPLETED
	android.permission.WRITE_EXTERNAL_STORAGE
	android.permission.INTERNET
	android.permission.ACCESS_NETWORK_STATE
	android.permission.WAKE_LOCK
	android.permission.WRITE_CONTACTS
	android.permission.READ_PHONE_STATE
	android.permission.DELETE_PACKAGES
## Sources: 50
	<org.json.JSONObject: int getInt(java.lang.String)>: 2
	<android.content.ContentResolver: android.database.Cursor query(android.net.Uri,java.lang.String[],java.lang.String,java.lang.String[],java.lang.String)>: 6
	<java.io.ByteArrayOutputStream: byte[] toByteArray()>: 3
	<android.telephony.SmsMessage: long getTimestampMillis()>: 1
	<android.net.Uri: android.net.Uri parse(java.lang.String)>: 9
	<java.util.Date: long getTime()>: 2
	<java.net.InetAddress: java.net.InetAddress getByName(java.lang.String)>: 3
	<java.net.URL: java.lang.String getPath()>: 3
	<java.net.URL: java.lang.String getHost()>: 8
	<java.text.DateFormat: java.lang.String format(java.util.Date)>: 1
	<android.telephony.TelephonyManager: java.lang.String getDeviceId()>: 2
	<android.content.res.Resources: android.content.res.AssetManager getAssets()>: 2
	<java.lang.reflect.Field: java.lang.Object get(java.lang.Object)>: 2
	<android.os.Bundle: java.lang.String getString(java.lang.String)>: 1
	<java.lang.String: byte[] getBytes()>: 23
	<android.telephony.TelephonyManager: java.lang.String getSimOperatorName()>: 3
	<android.net.ConnectivityManager: android.net.NetworkInfo getActiveNetworkInfo()>: 4
	<java.lang.Class: java.lang.reflect.Field[] getDeclaredFields()>: 1
	<android.view.View: int getId()>: 1
	<android.telephony.TelephonyManager: java.lang.String getLine1Number()>: 9
	<android.content.Intent: android.os.Bundle getExtras()>: 2
	<android.telephony.TelephonyManager: java.lang.String getSubscriberId()>: 1
	<java.io.BufferedReader: java.lang.String readLine()>: 3
	<java.lang.String: byte[] getBytes(java.lang.String)>: 1
	<android.net.NetworkInfo: android.net.NetworkInfo$State getState()>: 3
	<java.lang.Runtime: java.lang.Runtime getRuntime()>: 2
	<android.view.MotionEvent: int getAction()>: 1
	<java.lang.Class: java.lang.String getName()>: 1
	<android.content.Intent: android.content.Intent setClass(android.content.Context,java.lang.Class)>: 7
	<android.telephony.SmsMessage: java.lang.String getOriginatingAddress()>: 1
	<java.net.HttpURLConnection: int getResponseCode()>: 6
	<android.os.Environment: java.io.File getExternalStorageDirectory()>: 1
	<android.content.Intent: java.lang.String getAction()>: 2
	<java.net.Socket: java.io.OutputStream getOutputStream()>: 3
	<java.net.Socket: java.io.InputStream getInputStream()>: 2
	<android.telephony.SmsMessage: android.telephony.SmsMessage createFromPdu(byte[])>: 1
	<java.lang.Thread: java.lang.Thread$UncaughtExceptionHandler getDefaultUncaughtExceptionHandler()>: 1
	<java.net.URL: int getPort()>: 9
	<android.widget.EditText: android.text.Editable getText()>: 126
	<android.os.Environment: java.lang.String getExternalStorageState()>: 1
	<android.telephony.TelephonyManager: java.lang.String getSimSerialNumber()>: 4
	<java.io.File: java.lang.String getAbsolutePath()>: 12
	<java.lang.Throwable: java.lang.Throwable getCause()>: 2
	<java.lang.reflect.Field: java.lang.String getName()>: 2
	<android.telephony.SmsMessage: java.lang.String getDisplayMessageBody()>: 1
	<java.lang.Long: long parseLong(java.lang.String)>: 2
	<android.os.Bundle: java.lang.Object get(java.lang.String)>: 1
	<android.os.PowerManager: android.os.PowerManager$WakeLock newWakeLock(int,java.lang.String)>: 1
	<android.net.NetworkInfo: java.lang.String getTypeName()>: 1
	<java.lang.Integer: int parseInt(java.lang.String)>: 3
## Sinks: 30
	<java.lang.String: boolean startsWith(java.lang.String)>: 6
	<android.util.Log: int e(java.lang.String,java.lang.String,java.lang.Throwable)>: 4
	<android.content.Intent: android.content.Intent setAction(java.lang.String)>: 1
	<android.net.Uri: android.net.Uri parse(java.lang.String)>: 9
	<android.os.Handler: boolean sendMessage(android.os.Message)>: 1
	<java.io.FileOutputStream: void write(byte[],int,int)>: 4
	<android.content.ContentValues: void put(java.lang.String,java.lang.Integer)>: 2
	<android.content.Intent: android.content.Intent setClass(android.content.Context,java.lang.Class)>: 7
	<java.lang.Thread: void setDefaultUncaughtExceptionHandler(java.lang.Thread$UncaughtExceptionHandler)>: 1
	<java.lang.String: java.lang.String substring(int,int)>: 5
	<android.util.Log: int i(java.lang.String,java.lang.String)>: 84
	<android.util.Log: int d(java.lang.String,java.lang.String)>: 43
	<android.content.Intent: android.content.Intent setDataAndType(android.net.Uri,java.lang.String)>: 1
	<android.content.ContentValues: void put(java.lang.String,java.lang.String)>: 3
	<java.io.OutputStream: void write(byte[],int,int)>: 3
	<android.app.ProgressDialog: void setMessage(java.lang.CharSequence)>: 7
	<android.widget.TextView: void setText(java.lang.CharSequence)>: 1
	<android.app.ProgressDialog: void setIndeterminate(boolean)>: 3
	<android.content.Intent: android.content.Intent putExtra(java.lang.String,java.lang.String)>: 1
	<android.widget.RadioGroup: void setOnCheckedChangeListener(android.widget.RadioGroup$OnCheckedChangeListener)>: 1
	<java.net.URL: java.net.URLConnection openConnection()>: 5
	<java.io.OutputStream: void write(byte[])>: 17
	<android.content.res.AssetManager: java.io.InputStream open(java.lang.String)>: 2
	<java.lang.Long: long parseLong(java.lang.String)>: 2
	<java.lang.Integer: int parseInt(java.lang.String)>: 3
	<android.app.Activity: void onCreate(android.os.Bundle)>: 8
	<android.os.AsyncTask: void onPostExecute(java.lang.Object)>: 1
	<android.content.ContentValues: void put(java.lang.String,java.lang.Long)>: 1
	<android.util.Log: int e(java.lang.String,java.lang.String)>: 6
	<java.net.HttpURLConnection: void setRequestMethod(java.lang.String)>: 5
