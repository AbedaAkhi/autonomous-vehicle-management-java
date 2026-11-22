# Manual Testing Evidence (Original Assignment)

**Evidence source:** `TestCases_22001797.pdf` (original submission). The tests below were documented using screenshots. They were not rerun when creating this portfolio.

| Feature | Scenario shown | Reported result |
| --- | --- | --- |
| Cities | Add five locations and display the graph | Locations listed |
| Roads | Add weighted road connections | Connections displayed with distances |
| Invalid road | Enter a location absent from the graph | Appropriate not-found message |
| Neighbours | Query connections for an existing city | Connected cities displayed |
| Invalid neighbour | Query an absent city | Not-found message |
| Path existence | Check between connected cities | `true` displayed |
| Same-vertex path | Use the same origin and destination | `true` displayed |
| Invalid destination | Check a route to an absent city | `false` displayed |
| Vehicle insertion | Add multiple vehicles with different IDs | Vehicle records displayed |
| Duplicate ID | Attempt to add an existing vehicle ID | Duplicate-ID warning |
| Vehicle lookup | Search an existing and a missing ID | Matching record / not-found message |
| Distance sorting | Sort by distance to destination | Ascending order shown |
| Nearest vehicle | Query nearest recorded vehicle | Shortest-distance entry returned |
| Battery sorting | Sort by battery percentage | Descending order shown |
| Highest battery | Query top battery level | Highest-battery entry returned |
| Vehicle deletion | Delete a vehicle and repeat lookup/sorting | Removed vehicle absent and recommendations updated |

## Test-method limitations

- These are **manual demonstration scenarios**, not a JUnit or CI test suite.
- Screenshots in the supplied test report document selected inputs and outputs, but do not prove that every edge case was exhaustively covered.
- No current source code or runnable build artifacts were supplied, so the results have not been independently reverified.
