# Yoroi Configuration Repository

This repository contains configuration files used by both the Yoroi Extension and Yoroi Mobile applications.

## Structure

- `prod.json`: Main production configuration file.

## Usage

These configuration files are consumed by the Yoroi applications to manage various settings and parameters.

## Guidelines for Changes

When proposing changes to the configuration files, please adhere to the following guidelines:

1.  **Pull Requests (PRs):** All changes must be submitted via a Pull Request.
2.  **Synchronization:** Ensure that any changes made to the configuration are reflected and compatible with both the Yoroi Extension and Yoroi Mobile applications. Changes in this repository should ideally be coordinated with corresponding application updates.
3.  **Schema Changes & Backward Compatibility:**
    *   If a schema change is necessary, **do not modify existing property names or their expected data types.**
    *   Instead, introduce new properties with different names to accommodate the new schema. This ensures backward compatibility for older versions of the Yoroi Extension and Mobile applications that may still be using the previous schema.
    *   Old properties can be deprecated but should not be removed until all active application versions have been updated to use the new schema.