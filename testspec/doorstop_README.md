# Doorstop useful commands

## Item creation 
Create a parent requirement
```bash
doorstop create <prefix HWRQ/IPVS etc> <path> -i markdown -s -
```
Add a new requirement 
```bash
doorstop add <prefix PRQ/HWRQ/IPVS etc> -n <name>
```
Create a child requirement 
```bash
doorstop create <prefix HWRQ_BLK1 etc> <path> -i markdown -s - -p <prefix HWRQ/IPVS etc>
```
## Documentation
Any block diagram, waveform image etc shall be stored under each generated item's directory in a new directory named `assets`

## Export

### HTML
```bash
# From the unit/requirements directory execute
doorstop publish all ./html
```
### Markdown of individual item

```bash
# From the unit/requirements directory execute
doorstop publish <prefix HWRQ/IPVS etc> ./out/<name>.md
```
## Official documentation

https://doorstop.readthedocs.io/en/latest/
