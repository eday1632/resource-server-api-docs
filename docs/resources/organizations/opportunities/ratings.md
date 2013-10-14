# Resources

## Ratings on Opportunities

### Attributes

[See Rating attributes here.](/docs/resources/organizations/ratings.md)

### Endpoints

#### `GET resources/:resource_id/ratings`

Returns the aggregate ratings on an opportunity as an array (e.g. `[name: value, name2: value2]`).

#### `POST resources/:resource_id/ratings`

Creates a new rating.

#### `PUT resources/:resource_id/ratings/:id`

Updates a rating. The `:id` in this case is the `name` attribute, but the parameter name is `id`

#### `DELETE resources/:resource_id/ratings/:id`

Deletes a specific rating. The `:id` in this case is the `name` attribute, but the parameter name is `id`

### Permissions

* Anyone can add a rating on a resource.
* Only admins and the API client that submitted the original rating can update or delete it.