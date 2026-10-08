# nsODBCExt plug-in for NSIS

![License](https://img.shields.io/github/license/nsis-community/plugin-nsodbcext?color=blue&style=for-the-badge)
![Release](https://img.shields.io/github/v/release/nsis-community/plugin-nsodbcext?style=for-the-badge)
![CI](https://img.shields.io/github/actions/workflow/status/nsis-community/plugin-nsodbcext/ci.yml?style=for-the-badge)

This repository mirrors the nsODBCExt plug-in, which was previously hosted on the [NSIS wiki](https://nsis.sourceforge.io/). Its source has been rearranged so that it builds automatically; code changes are limited to build fixes.

nsODBCExt is a fork of [nsODBC](https://github.com/nsis-community/plugin-nsodbc) that takes the attributes as one semicolon-separated string (`DSN=XXX;UID=0x777`) and retries with the multi-string format SQL Server needs. The original shipped as `nsODBC.dll`; it is renamed here so both plug-ins can be installed side by side. Call it as `nsODBCExt::AddDSN` instead of `nsODBC::AddDSN`. It builds for the Unicode targets only.

**Are you the author?** You're welcome to take it over: [open an issue](https://github.com/nsis-community/plugin-nsodbcext/issues/new) and we'll transfer the repository to you.

## Installation

Download the installer or archive from the [Releases page](https://github.com/nsis-community/plugin-nsodbcext/releases).

If you downloaded the zip archive, extract it into your NSIS folder: it adds `nsODBCExt.dll` to `Plugins/<variant>/`.
