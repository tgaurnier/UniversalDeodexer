UniversalDeodexer
=================

--------------------------------------------------------------------------------
--------------------------Universal Deodexer for Bash---------------------------

WARNING:
	Make sure you have a PROPER backup of your rom before using this script,
	if you are unsure of what a proper backup is, then you probably shouldn't
	be doing this.

NOTE:
	It is recommended for you to have your phone booted into recovery with the
	system partition mounted, this script will simultaneously pull, deodex,
	and push files back to phone, and if certain files are pushed back with
	the phone booted to Android it can cause it to force restart, which may
	have unexpected results.

USES:
	deodex <filename-without-extension>
		This will detect where the file is located on the phone, then it will
		pull and deodex the file, then push the file back, and delete the
		odex file from the phone.

		Example: deodex SystemUI

	deodex --all
		This will attempt to pull, deodex, then push back all odexed files on
		the phone, then it will delete all odex files from phone.

	deodex --restore
		This will attempt to push all original packages with odex files back
		to phone, restoring it to it's odexed condition.

--------------------------------------------------------------------------------