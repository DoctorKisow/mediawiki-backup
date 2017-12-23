# MediaWiki Backup

**mediawiki-backup** - A backup script for a MySQL based MediaWiki environment.<br />
Copyright &copy; 2015-2017, Matthew R. Kisow, D.Sc. <matthew.kisow@kisow.org>

## Tasks
- [ ] Modify the cron_management function:
```script
     from:
          /usr/sbin/mediawiki-backup -b -C -l
     
     to:
          bash -c "/usr/sbin/mediawiki-backup -b -C -l"
```
- [ ] Create a clobber/no-clobber flag for unattended backups.

## Installation
1. Following the instructions for your distribution, install git.
2. Using the _git clone_ command, clone **mediawiki-backup** from this repository into your home directory.
```shell
          cd ~
          git clone https://github.com/DoctorKisow/mediawiki-backup.git
```
3. Using the _chmod +x_ command, make the **mediawiki-backup** script executable.
```shell
          chmod +x mediawiki-backup
```
4. Using the _bash_ command, install **mediawiki-backup** using the -i switch.
```shell
          bash mediawiki-backup -i
```
5. using the _mediawiki-backup_ command, configure **mediawiki-backup** using the -c switch.
```shell
          mediawiki-backup -c
```

## Script Notes
By typing _mediawiki-backup_ with no options, or _mediawiki-backup -h_ you can get help.

## Warning
Do not use this script in a _PRODUCTION_ enviornment with out testing and validating it first.

## License
License (GPL v3.0)

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
