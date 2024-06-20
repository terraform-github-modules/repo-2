<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.6 |
| <a name="requirement_github"></a> [github](#requirement\_github) | 6.2.1 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_github"></a> [github](#provider\_github) | 6.2.1 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [github_repository.this](https://registry.terraform.io/providers/integrations/github/6.2.1/docs/resources/repository) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_allow_auto_merge"></a> [allow\_auto\_merge](#input\_allow\_auto\_merge) | (Optional) Set to true to allow auto-merging pull requests on the repository | `bool` | `null` | no |
| <a name="input_allow_merge_commit"></a> [allow\_merge\_commit](#input\_allow\_merge\_commit) | (Optional) Set to false to disable merge commits on the repository | `bool` | `null` | no |
| <a name="input_allow_rebase_merge"></a> [allow\_rebase\_merge](#input\_allow\_rebase\_merge) | (Optional) Set to false to disable rebase merges on the repository | `bool` | `null` | no |
| <a name="input_allow_squash_merge"></a> [allow\_squash\_merge](#input\_allow\_squash\_merge) | (Optional) Set to false to disable squash merges on the repository | `bool` | `null` | no |
| <a name="input_delete_branch_on_merge"></a> [delete\_branch\_on\_merge](#input\_delete\_branch\_on\_merge) | (Optional) Automatically delete head branch after a pull request is merged. Defaults to false | `bool` | `null` | no |
| <a name="input_description"></a> [description](#input\_description) | (Optional) A description of the repository | `string` | `null` | no |
| <a name="input_has_discussions"></a> [has\_discussions](#input\_has\_discussions) | (Optional) Set to true to enable GitHub Discussions on the repository. Defaults to false | `bool` | `null` | no |
| <a name="input_has_issues"></a> [has\_issues](#input\_has\_issues) | (Optional) Set to true to enable the GitHub Issues features on the repository | `bool` | `null` | no |
| <a name="input_has_projects"></a> [has\_projects](#input\_has\_projects) | (Optional) Set to true to enable the GitHub Projects features on the repository. Per the GitHub documentation when in an organization that has disabled repository projects it will default to false and will otherwise default to true. If you specify true when it has been disabled it will return an error | `bool` | `null` | no |
| <a name="input_has_wiki"></a> [has\_wiki](#input\_has\_wiki) | (Optional) Set to true to enable the GitHub Wiki features on the repository | `bool` | `null` | no |
| <a name="input_homepage_url"></a> [homepage\_url](#input\_homepage\_url) | (Optional) URL of a page describing the project | `string` | `null` | no |
| <a name="input_is_template"></a> [is\_template](#input\_is\_template) | (Optional) Set to true to tell GitHub that this is a template repository | `bool` | `null` | no |
| <a name="input_merge_commit_message"></a> [merge\_commit\_message](#input\_merge\_commit\_message) | (Optional) Can be PR\_BODY, PR\_TITLE, or BLANK for a default merge commit message. Applicable only if allow\_merge\_commit is true | `string` | `null` | no |
| <a name="input_merge_commit_title"></a> [merge\_commit\_title](#input\_merge\_commit\_title) | (Optional) Can be PR\_TITLE or MERGE\_MESSAGE for a default merge commit title. Applicable only if allow\_merge\_commit is true | `string` | `null` | no |
| <a name="input_name"></a> [name](#input\_name) | (Required) The name of the repository | `string` | n/a | yes |
| <a name="input_squash_merge_commit_message"></a> [squash\_merge\_commit\_message](#input\_squash\_merge\_commit\_message) | (Optional) Can be PR\_BODY, COMMIT\_MESSAGES, or BLANK for a default squash merge commit message. Applicable only if allow\_squash\_merge is true | `string` | `null` | no |
| <a name="input_squash_merge_commit_title"></a> [squash\_merge\_commit\_title](#input\_squash\_merge\_commit\_title) | (Optional) Can be PR\_TITLE or COMMIT\_OR\_PR\_TITLE for a default squash merge commit title. Applicable only if allow\_squash\_merge is true | `string` | `null` | no |
| <a name="input_visibility"></a> [visibility](#input\_visibility) | (Optional) Can be public or private. If your organization is associated with an enterprise account using GitHub Enterprise Cloud or GitHub Enterprise Server 2.20+, visibility can also be internal. The visibility parameter overrides the private parameter | `string` | `null` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_repository_id"></a> [repository\_id](#output\_repository\_id) | The ID of the bucket. |
<!-- END_TF_DOCS -->