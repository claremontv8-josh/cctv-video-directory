# CCTV Video Directory

A WordPress plugin for searching and browsing Claremont Community Television’s video catalog and linking to related School Board Meeting Navigator pages.

This standalone repository contains Kevin Tyson’s original plugin, extended by Kevin Tyson and Joshua Nelson. The plugin is licensed under **GNU GPL version 2 or, at your option, any later version**; see [LICENSE](LICENSE).

## Install

The plugin requires WordPress 6.2 or newer and PHP 7.4 or newer. For WordPress upload and packaging instructions, see [readme.txt](readme.txt).

## Embed

Use <code>[cctv_directory]</code> for the full video directory.

For a compact homepage embed, use <code>[cctv_directory mode="home"]</code>. In Divi, add a **Shortcode** module; in the WordPress block editor, add a **Shortcode** block. This mode starts with one responsive row (6 videos on desktop, 3 on tablet, 1 on phone). **List more rows** expands the results, search and filters update results in place, and video links open in a new tab.

## Catalog refresh

The plugin ships with a catalog snapshot so it can display videos immediately. After activation, WordPress schedules source refreshes daily. WordPress Cron is traffic-triggered, so low-traffic sites may run refreshes later than scheduled; configure a server cron for wp-cron.php if reliable timing is needed.

Visitors’ browsers may keep a saved catalog copy and show an update notice when a newer catalog is available. Administrators can start a refresh from **Settings → CCTV Directory**.

## Data sources

The plugin retrieves public program metadata from CCTV and meeting-page links from the Claremont School Board Meeting Navigator. It does not copy or host the video recordings.

## Authors

Kevin Tyson created the original plugin. Kevin Tyson and Joshua Nelson contributed the subsequent functionality and interface changes.

