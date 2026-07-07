Flow Functionality:

Accepts a product ID from the incoming request.
Checks whether inventory data is already available in the cache.
Returns the cached inventory immediately when available.
Retrieves the latest inventory information when the cache does not contain the requested product.
Stores newly retrieved inventory in the cache for future requests.
Returns appropriate responses when the product is unavailable in both the cache and the source system.

Error Handling:

The application includes comprehensive error handling to ensure reliable execution under different failure scenarios.
Validates mandatory request parameters before processing.
Handles invalid requests with meaningful validation messages.
Detects database connectivity and query execution failures while accessing the cache.
Handles failures while retrieving inventory from the source system.
Prevents unexpected system failures from exposing internal exceptions.
Returns standardized error responses with appropriate status codes and descriptive messages.
Logs all business and technical errors to simplify monitoring and troubleshooting.
