# Logger
Dvsa FTTS uses Winston as the logging facade.

## Usage
Firstly, install the library
```
npm install @dvsa/azure-logger
```

or if using Yarn

```
yarn add @dvsa/azure-logger
```

Specify the environment variables in an .env file, for example

```
LOG_LEVEL=debug
NODE_ENV=development
```

Import the logger (singleton instance)
```typescript
import { logger } from '@dvsa/azure-logger';

// do some logging!
logger.log('Hello World');
logger.error('Error %o', err);
```

### Logging levels
 * critical
 * error
 * warn
 * info
 * debug
 * security
 * audit
 * log
