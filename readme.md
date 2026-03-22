

### ❤️ FIX src/index.ts line 1554:


// Use sourceId as key, and merge all busses from all addresses
				if (!tallyData[source.id]) {
					tallyData[source.id] = []
				}
				// Merge busses, avoiding duplicates
				for (const bus of busses) {
					if (!tallyData[source.id].includes(bus)) {
						tallyData[source.id].push(bus)
					}
				}
