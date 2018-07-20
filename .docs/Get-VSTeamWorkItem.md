<!-- #include "./common/header.md" -->

# Get-VSTeamWorkItem

## SYNOPSIS

<!-- #include "./synopsis/Get-VSTeamWorkItem.md" -->

## SYNTAX

## DESCRIPTION

<!-- #include "./synopsis/Get-VSTeamWorkItem.md" -->

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------

```PowerShell
PS C:\> Get-VSTeamWorkItem -ProjectName demo -Ids 47,48
```

This command gets work items with IDs 47 and 48 by using the ID parameter.

## PARAMETERS

<!-- #include "./params/projectName.md" -->

### -Id

The id of the work item.

```yaml
Type: Int32
Parameter Sets: ByID
Required: True
Accept pipeline input: true (ByPropertyName, ByValue)
```

### -Ids

The id of the work item.

```yaml
Type: Int32[]
Parameter Sets: List
Required: True
Accept pipeline input: true (ByPropertyName, ByValue)
```

### -ErrorPolicy

The flag to control error policy in a bulk get work items request.  The acceptable values for this parameter are:

- Fail
- Omit

```yaml
Type: String
Parameter Sets: List
Required: True
Default value: Fail
```

### -Fields

Comma-separated list of requested fields.

```yaml
Type: String[]
```

### -Expand

Comma-separated list of requested fields.  The acceptable values for this parameter are:

- None
- Relations
- Fields
- Links
- All

```yaml
Type: String
```

### -AsOf

```yaml
Type: DateTime
```

## INPUTS

### System.String

ProjectName

WorkItemType

## OUTPUTS

## NOTES

WorkItemType is a dynamic parameter and use the default project value to query their validate set.

If you do not set the default project by called Set-VSTeamDefaultProject before calling Get-VSTeamWorkItem you will have to type in the names.

## RELATED LINKS