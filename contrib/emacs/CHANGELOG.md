# 2.3.3

* (cleanup) Avoid double decryption and reduce the scope of
  `inhibit-message` in internal functions.

# 2.3.2

* (bugfix) Ensure the system clipboard is cleared after
  the timeout expired.

# 2.3.1

* (bug) Drop dependency on s library.

# 2.3.0

* (bug) Drop auth-source-pass dependency.
  Bump Emacs minor version requirement to emacs 26.

# 2.2.0

* (feature) Add command password-store-generate-no-symbols

# 2.1.5

* (bugfix) Fix an infloop on Windows enviroments.

# 2.1.4

* Drop dependency on f library.

# 2.1.3

* Update password-store-clear docstring; clarify that the
  optional argument is only used in the print out message.

# 2.1.2

* Make argument optional in password-store-clear to preserve
  backward compatibility.

# 2.1.1

* (bugfix) Check that auth-source-pass-filename is bound before use it.

# 2.1.0

* (feature) Support extraction of any secret fields stored in the files.

* (feature) The library is now integrated with auth-source-pass; thus, the
            filename of the password-store folder is set with the option
            auth-source-pass-filename.

# 2.0.5

Improve password-store-insert message on success/failure

# 2.0.4
	
* Re add password-store-timeout function to preserve backward
  compatibility with other libraries relying on it.
	
# 2.0.3
	
* (feature) Update password-store-password-length default value to 25
	
* (feature) Add option password-store-time-before-clipboard-restore; delete
            password-store-timeout and use the new option instead.
	
# 1.0.2

* (bugfix) Fix typo in password-store-url function doc string

# 1.0.1

* (bugfix) Quote shell arguments in async call

# 1.0.0

* (feature) Call `pass edit` so that changes get committed to git

# 0.1

* Initial release
