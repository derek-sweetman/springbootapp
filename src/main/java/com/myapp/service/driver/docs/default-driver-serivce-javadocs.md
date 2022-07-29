# Documentation

## `@Service public class DefaultDriverService implements DriverService`

Service to encapsulate the link between DAO and controller and to have business logic for some driver specific things. <p/>

## `@Override @Transactional public DriverDO find(Long driverId) throws EntityNotFoundException`

Selects a driver by id.

 * **Parameters:** `driverId` — 
 * **Returns:** found driver
 * **Exceptions:** `EntityNotFoundException` — if no driver with the given id was found.

## `@Override @Transactional public DriverDO create(DriverDO driverDO) throws ConstraintsViolationException`

Creates a new driver.

 * **Parameters:** `driverDO` — 
 * **Returns:** 
 * **Exceptions:** `ConstraintsViolationException` — if a driver already exists with the given username, ... .

## `@Override @Transactional public void delete(Long driverId) throws EntityNotFoundException`

Deletes an existing driver by id.

 * **Parameters:** `driverId` — 
 * **Exceptions:** `EntityNotFoundException` — if no driver with the given id was found.

## `@Override @Transactional public void updateLocation(long driverId, double longitude, double latitude) throws EntityNotFoundException, ConstraintsViolationException`

Update the location for a driver.

 * **Parameters:**
   * `driverId` — 
   * `longitude` — 
   * `latitude` — 
 * **Exceptions:** `EntityNotFoundException` — 

## `@Override public List<DriverDO> find(OnlineStatus onlineStatus)`

Find all drivers by online state.

 * **Parameters:** `onlineStatus` — 
