---
name: Create a fork
example: octokit.rest.repos.createFork({ owner, repo })
route: POST /repos/{owner}/{repo}/forks
scope: repos
type: API method
---

# Create a fork

Create a fork for the authenticated user.

**Note**: Forking a Repository happens asynchronously. You may have to wait a short period of time before you can access the git objects. If this takes longer than 5 minutes, be sure to contact [GitHub Support](https://support.github.com/contact?tags=rest-api).

```js
octokit.rest.repos.createFork({
  owner,
  repo,
});
```

## Parameters

<table>
  <thead>
    <tr>
      <th>name</th>
      <th>required</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>owner</td><td>yes</td><td>

</td></tr>
<tr><td>repo</td><td>yes</td><td>

</td></tr>
<tr><td>organization</td><td>no</td><td>

Optional parameter to specify the organization name if forking into an organization.

</td></tr>
  </tbody>
</table>

See also: [GitHub Developer Guide documentation](https://docs.github.com/rest/reference/repos#create-a-fork).
