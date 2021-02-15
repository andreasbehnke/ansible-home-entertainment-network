# This repository is outdated and only available for documentation purposes. The only maintained ansible repsoitories are these prefixed with ansible_role_XYZ

# Home Entertainment Network

Purpose of this ansible project is to provide playbooks for members of a home entertainment network. The network consist of the following members:

 * homeserver
   This singleton instance provides a TV video recorder and file shares for different media types.
   The following software will be installed:
   - VDR with VNSI plugin for streaming clients
   - Live plugin for VDR to manage video recorder with webfrontend
   - Samba for providing read/write access to media shares

 * media_clients
   A media center software to play back media provided by homeserver. These clients are either OSMC based raspberry pi devices or Ubuntu based desktop clients.
   The following software will be installed:
   - Kodi with VNSI PVR plugin for streaming live TV from homeserver
   - Configured to access media shares of homeserver

 * media_management_clients
   A client which is able to manage photos and videos on homeserver.
   The following software will be installed:
   - rapid photo downloader for uploading private media like photos and videos from smartphones to homeserver
   - video transcoding tool handbrake
