# shell_utils
1. expect_example： A simple example for how to use expect tools, so we could execute CMD on remote machine.
Three parameters are required to execute the script, such as remote machine's user name, host ip, and user password.
The following are examples of using PHP:
```
		$expect_path = '/usr/bin/expect'; // expect path
		$expect_example_script = ' '; // expect_example script path
		$userName = ' '; // remote machine's user name
		$hostIp = ' '; // remote machine's host ip
		$adminPasswd = ' '; // remote machine's user password
		$exec_expect_example = sprintf ( "%s %s %s %s %s", $expect_path, $expect_example_script, $userName, $hostIp, $adminPasswd);
		exec($expect_example_script, $temp_data, $ret);	
```
