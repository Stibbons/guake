=====
Guake
=====

.. _Guake_(unreleased yet):

(unreleased yet)
================

.. _Guake_(unreleased yet)_Bug Fixes:

Bug Fixes
---------

.. releasenotes/notes/fix-preference-window-header-color,-align-close-button-and-change-borders-to-margins-fa7ffffc45b12ea5.yaml @ b'2333606e7af3deb165bc8de23c392472420cf163'

- fix preferences window header color, align the close button more nicely and change borders to margins


.. _Guake_3.0.4:

3.0.4
=====

.. _Guake_3.0.4_New Features:

New Features
------------

.. releasenotes/notes/Add-window-displacement-options-to-move-guake-away-from-the-edges-1b2d46997e8dbe91.yaml @ b'93099961f7c90a22089b76a8a9acf1414bea56e5'

- Add window displacement options to move guake away from the screen edges

.. releasenotes/notes/Add-window-displacement-options-to-move-guake-away-from-the-edges-1b2d46997e8dbe91.yaml @ b'93099961f7c90a22089b76a8a9acf1414bea56e5'

- User can manually enter the name of the GTK theme it wants Guake to use. Note there is no
  Preference settings yet, one needs to manually enter the name using ``dconf-editor``, in the
  key ``/apps/guake/general/gtk-theme-name``. Use a name matching one the folders in
  ``/usr/share/themes``. Please also considere this is a early adopter features and has only
  been tested on Ubuntu systems.
  Dark theme preference can be se with the key ``/apps/guake/general/gtk-prefer-dark-theme``.

.. releasenotes/notes/fix-make-install-system-as-non-root-user-40cdbb0509660741.yaml @ b'7fb39459c9dd852411fcd968fcfbbf33f5bfa4ca'

- Allow make install-system to be run as non root user and print a message if so.

.. releasenotes/notes/quick_open-032209b39bb6831f.yaml @ b'4423af1c134e80a81e4c68fdcf5eea2ade969c74'

- Quick open can now open file under selection. Simply select a filename in the current terminal
  and do a Ctrl+click, if the file path can be found, it will be open in your editor. It allows
  to virtually open any file path in your terminal (if they are on your local machine), but
  requires the user to select the file path first, compared to the Quick Open feature that
  finds file names using regular expression.
  
  Also notes that is it able to look in the current folder if the selected file name exists,
  allowing Ctrl+click on relative paths as well.
  
  Line number syntax is also supported: ``filename.txt:5`` will directly on the 5th line if
  your Quick Open is set for.


.. _Guake_3.0.4_Bug Fixes:

Bug Fixes
---------

.. releasenotes/notes/Add-window-displacement-options-to-move-guake-away-from-the-edges-1b2d46997e8dbe91.yaml @ b'93099961f7c90a22089b76a8a9acf1414bea56e5'

- fixes issue with vertically stacked dual monitors #1162

.. releasenotes/notes/bugfix-654583b5646cf905.yaml @ b'1367a6b7cdf856efea50e0956f894be088d1f681'

- Quick Open functionnality is restored #1121

.. releasenotes/notes/bugfix-90bd70c984ad6a73.yaml @ b'69ae4fe8036eae8e2f7418cd08fccb95fe41eb07'

- Unusable Guake with "hide on focus lose" option #1152

.. releasenotes/notes/dbus-c3861541c24b328a.yaml @ b'c0443dd7df49346a87f1fa08a52c1c6f76727ad8'

- Speed up guake D-Bus communication (command line such as ``guake -t``).


.. _Guake_3.0.3:

3.0.3
=====

.. _Guake_3.0.3_Release Summary:

Release Summary
---------------

.. releasenotes/notes/gtk3-a429d01811754c42.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

This minor release mainly focus on fixing big problems that was remaining after the migration to GTK3. I would like to akwonledge the work of some contributors that helped testing and reporting issues on Guake 3.0.0. Thanks a lot to @egmontkob and @aichingm.


.. releasenotes/notes/prefs-032d2ab0c8e2f17a.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

The Preference window has been deeply reworked and the hotkey management has been rewriten. This was one the the major regression in Guake 3.0.


.. _Guake_3.0.3_New Features:

New Features
------------

.. releasenotes/notes/auto-edit-648e3609c9aee103.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- [dev env] automatically open reno slug after creation for editing

.. releasenotes/notes/dev-env-fb2967d1ba8ee495.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- [dev env]: Add the possibility to terminate guake with ``Ctrl+c`` on terminal
  where Guake has been launched

.. releasenotes/notes/scroll-959087c80640ceaf.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Add "Infinite scrolling" option in "Scrolling" panel #274

.. releasenotes/notes/show-focus-cab5307b44905f7e.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Added hotkey for showing and focusing Guake window when it is opened or closed.
  It is convenient when Guake window are overlapped with another windows and user
  needs to just showing it without closing and opening it again. #1133


.. _Guake_3.0.3_Known Issues:

Known Issues
------------

.. releasenotes/notes/packages-55d1017dd708b8de.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Quick Edit feature is not working (#1121)


.. _Guake_3.0.3_Deprecations:

Deprecations
------------

.. releasenotes/notes/visible-bell-12de7acf136d3fa4.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Remove visible bell feature #1081


.. _Guake_3.0.3_Bug Fixes:

Bug Fixes
---------

.. releasenotes/notes/fix-guake-showing-up-on-startup-0fdece37dc1616e4.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Command options do not work, crash when disabling keybinding #1111

.. releasenotes/notes/fix-guake-showing-up-on-startup-0fdece37dc1616e4.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Do not open Guake window upon startup #1113

.. releasenotes/notes/fix-in/decrease-height-8176a8313d9a1aba.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Fix crash on increase/decrease main window height shortcut #1099

.. releasenotes/notes/fix-rename-tab-shortcut-62ad1410c2958929.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Resolved conflicting default shortcut for ``Ctrl+F2`` (now, rename current tab is set to
  ``Ctrl+Shift+R``) #1101, #1098

.. releasenotes/notes/hotkeys-42708e8968fd7b25.yaml @ b'41c5b8b408b0360483f2e467f616f88a534acf83'

- The hotkey management has been rewriten and is now fully functional

.. releasenotes/notes/prefs-032d2ab0c8e2f17a.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Rework the Preference window and reorganize the settings. Lot of small issues
  has been fixed.
  The Preference window now fits in a 1024x768 screen.

.. releasenotes/notes/run-command-517683bd988aa06a.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Fix 'Failed to execute child process "-"' - #1119

.. releasenotes/notes/scroll-959087c80640ceaf.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- History size spin is fixed and now increment by 1000 steps. Default history value is now set to
  1000, because "1024" has no real meaning for end user. #1082


.. _Guake_3.0.3_Translation Updates:

Translation Updates
-------------------

.. releasenotes/notes/translation-31e67dc4190a9067.yaml @ b'7cb971cf125e41f6294b8b17003276abb18a8734'

- de

.. releasenotes/notes/translation-31e67dc4190a9067.yaml @ b'7cb971cf125e41f6294b8b17003276abb18a8734'

- fr

.. releasenotes/notes/translation-31e67dc4190a9067.yaml @ b'7cb971cf125e41f6294b8b17003276abb18a8734'

- ru


.. _Guake_3.0.3_Other:

Other
-----

.. releasenotes/notes/packages-55d1017dd708b8de.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- The dependencies of the Guake executable has been slightly better described in README.
  There is an example for Debian/Ubuntu in the file ``bootstrap-dev-debian.sh`` which is the main
  environment where Guake is developed and tested.

.. releasenotes/notes/packages-55d1017dd708b8de.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Package maintainers are encouraged to submit their ``bootstrap-dev-[distribution].sh``,
  applicable for other distributions, to help users install Guake from source, and other package
  maintainers.


.. _Guake_3.0.2:

3.0.2
=====

.. _Guake_3.0.2_New Features:

New Features
------------

.. releasenotes/notes/dark_theme-4bb6be4b2cfd92ae.yaml @ b'b0f73e5d93f3b688cf311f5925eb0c95d8cc64e4'

- Preliminary Dark theme support. To use it, install the 'numix' theme in your system.
  For example, Ubuntu/Debian users would use ``sudo apt install numix-gtk-theme``.


.. _Guake_3.0.2_Known Issues:

Known Issues
------------

.. releasenotes/notes/dark_theme-4bb6be4b2cfd92ae.yaml @ b'b0f73e5d93f3b688cf311f5925eb0c95d8cc64e4'

- Cannot enable or disable the GTK or Dark theme by a preference setting.


.. _Guake_3.0.2_Deprecations:

Deprecations
------------

.. releasenotes/notes/resizer-d7c6553879852019.yaml @ b'4b50f6714f56e72b38856ec1933790c5624e3399'

- Resizer discontinued


.. _Guake_3.0.2_Bug Fixes:

Bug Fixes
---------

.. releasenotes/notes/make-096ad37e6079df09.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Fix ``sudo make uninstall/install`` to work only with ``/usr/local``

.. releasenotes/notes/make-096ad37e6079df09.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Fix translation ``mo`` file generation

.. releasenotes/notes/make-096ad37e6079df09.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- Fix crash on Wayland

.. releasenotes/notes/match-b205323a7aa019f9.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Fix quick open and open link in terminal

.. releasenotes/notes/not_composited_de-505082d1c18eda3c.yaml @ b'6459a2c14fd5366fae5d245aac9df21e7e7955dc'

- Fixed Guake initialization on desktop environment that does not support compositing.


.. _Guake_3.0.1:

3.0.1
=====

.. _Guake_3.0.1_Release Summary:

Release Summary
---------------

.. releasenotes/notes/maintenance-e02e946e15c940ab.yaml @ b'5cbf4cf065f11067118430eda32cb2fcb5516874'

Minor maintenance release.


.. _Guake_3.0.1_Bug Fixes:

Bug Fixes
---------

.. releasenotes/notes/maintenance-e02e946e15c940ab.yaml @ b'5cbf4cf065f11067118430eda32cb2fcb5516874'

- Code cleaning and GNOME desktop file conformance


.. _Guake_3.0.0:

3.0.0
=====

.. _Guake_3.0.0_Release Summary:

Release Summary
---------------

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

Guake has been ported to GTK-3 thanks to the huge work of @aichingm. This also implies Guake now uses the latest version of the terminal emulator component, VTE 2.91.
Guake is now only working on Python 3 (version 3.5 or 3.6). Official support for Python 2 has been dropped.
This enables new features in upcoming releases, such as "find in terminal", or "split screen".


.. _Guake_3.0.0_New Features:

New Features
------------

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Ported to GTK3:
  
    - cli arguments
    - D-Bus
    - context menu of the terminal, the tab bar and the tray icon
    - scrollbar of the terminal
    - ``ctrl+d`` on terminal
    - fix double click on the tab bar
    - fix double click on tab to rename
    - fix clipboard from context menu
    - notification module
    - keyboard shortcuts
    - preference screen
    - port ``gconfhandler`` to ``gsettingshandler``
    - about dialog
    - pattern matching
    - ``Guake.accel*`` methods

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Guake now use a brand new build system:
  
    - ``pipenv`` to manage dependencies in `Pipfile`
    - enforced code styling and checks using Pylint, Flake8, Yapf, ISort.
    - simpler release management thanks to PBR

.. releasenotes/notes/reno-3b5ad9829b256250.yaml @ b'8ea70114fc51ffef8436da8cde631a8246cc6794'

- [dev env] `reno <https://docs.openstack.org/reno/latest/>`_ will be used to generate
  release notes for Guake starting version 3.0.0.
  It allows developers to write the right chunk that will appear in the release
  note directly from their Pull Request.

.. releasenotes/notes/update-window-title-c6e6e3917821902d.yaml @ b'5f6952a8385f93bfc649b434b6e4728b046f714d'

- Update Guake window title when:
    - the active tab changes
    - the active tab is renamed
    - the vte title changes


.. _Guake_3.0.0_Known Issues:

Known Issues
------------

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Translation might be broken in some language, waiting for the translation file to be updated by volunteers

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Resizer does not work anymore

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Package maintainers have to rework their integration script completely

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- quick open and open link in terminal is broken

.. releasenotes/notes/update-window-title-c6e6e3917821902d.yaml @ b'5f6952a8385f93bfc649b434b6e4728b046f714d'

- **Note for package maintainers**: Guake 3 has a minor limitation regarding Glib/GTK Schemas
  files. Guake looks for the gsettings schema inside its data directory. So you will probably
  need install the schema twice, once in ``/usr/local/lib/python3.5/dist-packages/guake/data/``
  and once in ``/usr/share/glib-2.0/schemas`` (see
  `#1064 <https://github.com/Guake/guake/issues/1064>`_).
  This is planned to be fixed in Guake 3.1


.. _Guake_3.0.0_Upgrade Notes:

Upgrade Notes
-------------

.. releasenotes/notes/pref-af8621e5c04d973c.yaml @ b'5f6952a8385f93bfc649b434b6e4728b046f714d'

- Minor rework of the preference window.


.. _Guake_3.0.0_Deprecations:

Deprecations
------------

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Background picture is no more customizable on each terminal

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- Visual Bell has been deprecated


.. _Guake_3.0.0_Translation Updates:

Translation Updates
-------------------

.. releasenotes/notes/gtk3-800a345dfd067ae6.yaml @ b'dcb33c0f7048f5c96c2d13f747bbd686c65dd91d'

- fr-FR

