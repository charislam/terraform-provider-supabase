---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "supabase_branch Resource - terraform-provider-supabase"
subcategory: ""
description: |-
  Branch database resource
---

# supabase_branch (Resource)

Branch database resource

## Example Usage

```terraform
resource "supabase_branch" "new" {
  parent_project_ref = "mayuaycdtijbctgqbycg"
  git_branch         = "main"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `git_branch` (String) Git branch
- `parent_project_ref` (String) Parent project ref

### Optional

- `region` (String) Database region

### Read-Only

- `database` (Attributes) Database connection details (see [below for nested schema](#nestedatt--database))
- `id` (String) Branch identifier

<a id="nestedatt--database"></a>
### Nested Schema for `database`

Read-Only:

- `host` (String) Host
- `id` (String) Branch project ref
- `jwt_secret` (String, Sensitive) JWT secret
- `password` (String, Sensitive) Password
- `port` (Number) Port
- `status` (String) Status
- `user` (String) User
- `version` (String) Postgres version