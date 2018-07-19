# node-clinic-doctor-examples

Server examples for `clinic`

```
git clone git@github.com:nearform/node-clinic-doctor-examples.git
cd node-clinic-doctor-examples
npm install
npm install -g clinic
npm install -g autocannon
```

## Examples

### Event Loop

```
clinic doctor --on-port 'autocannon localhost:$PORT' -- node slow-event-loop
```

### GC

```
clinic doctor --on-port 'autocannon localhost:$PORT -c 2500' -- node slow-gc
```

### I/O

```
clinic doctor --on-port 'autocannon localhost:$PORT' -- node slow-io
```

### Sync I/O

```
clinic doctor --on-port 'autocannon localhost:$PORT' -- node sync-io
```

## License

[Apache 2.0](<https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)>)
