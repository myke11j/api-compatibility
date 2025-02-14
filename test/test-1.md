Develop a program that retrieves data from two different sources:
1. **Historical Data** - Previously retrieved data stored in files within the `data/*` directory, which was originally fetched from `v1_api`.
2. **New Data** - Fresh data obtained from `v2_api`.

The program should **merge the data** by adding only the `value` field from `v2_api` to the corresponding records in `v1_api` data. The merged data should then be saved to a file for further use.

**Requirements**

- **Data Handling:** Instead of making actual API calls during this test, the program should read from files in the `data/*` directory.
- **Live API Mode:** Implement a toggle (e.g., a command-line flag or a configuration setting) to switch between reading from files (test mode) and making actual API calls (live mode).
- **Merging Logic:** The program should ensure that only the `value` field from `v2_api` is added to the appropriate records in `v1_api` data, without altering other fields.
