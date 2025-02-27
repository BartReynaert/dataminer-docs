---
uid: Cube_Feature_Release_10.2.11
---

# DataMiner Cube Feature Release 10.2.11 – Preview

> [!IMPORTANT]
> We are still working on this release. Some release notes may still be modified or moved to a later release. Check back soon for updates!

> [!TIP]
> For release notes for this release that are not related to DataMiner Cube, see [General Feature Release 10.2.11](xref:General_Feature_Release_10.2.11).

## Highlights

*No highlights have been selected for this release yet*

## Other features

#### DataMiner Cube - Resources app: Removing resources from all pools [ID_34311]

<!-- Main Release Version 10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When you move one or more resources from a pool to the *(uncategorized)* pool, a confirmation box will now appear to warn you that, if you click *Yes*, the resources in question will be removed from all pools.

## Changes

### Enhancements

#### DataMiner Cube - Service & Resource Management: Function resource icons are now centered in service definition diagrams [ID_34249]

<!-- Main Release Version 10.2.0 [CU8] - Feature Release Version 10.2.11 -->

In service definition diagrams, function resource icons are now centered.

#### DataMiner Cube - Automation: Changes made to a script by other users will immediately be shown when selecting that script [ID_34277]

<!-- Main Release Version 10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When you select an unmodified Automation script in the Automation app, from now on, changes made to that script by other users (e.g. in another Cube session or in DataMiner Integration Studio) will immediately be shown.

#### Trending - Behavioral anomaly detection: Enhanced flatline detection [ID_34319]

<!-- MR 10.3.0 - FR 10.2.11 -->
<!-- Not added to 10.3.0 -->

A number of enhancements have been made with regard to the detection of change points of type "flatline".

#### DataMiner Cube - Visual Overview: Service context of a linked shape will only be determined when the service context has been specified [ID_34340]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When a shape was linked to an element that was not part of a service, up to now, an attempt would be made to determine the service context even when no service context had been specified. From now on, the service context will only be determined when the service context has been specified in the shape.

#### DataMiner Cube - Visual Overview: Enhanced performance when sorting dynamically positioned shapes [ID_34351]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

Because of a number of enhancements, overall performance has increased when sorting dynamically positioned shapes.

#### DataMiner Cube - Visual Overview: Caching of user settings in order to enhanced performance [ID_34383]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

In Visual Overview, the current value of the following user settings will now be cached in order to enhance performance:

- *Open element cards undocked* (*Settings* window)
- *AlarmSettings.Blinking* (*MaintenanceSettings.xml* file)

#### DataMiner Cube - Visual Overview: Enhanced performance when determining whether a shape is clickable [ID_34386]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

A number of enhancements have been made to the procedure called to determine whether a shape is clickable.

### Fixes

#### DataMiner Cube - Trending: Y axis would incorrectly show other values when the trend graph showed a constant exception value [ID_34242]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When you opened a trend graph that only showed a constant exception value, the Y axis would incorrectly not only show the exception value but also a number of other values. In cases like this, from now on, the Y axis will only show the exception value.

#### DataMiner Cube - Trending: Y-axis values did not take into account the number of decimals configured in the protocol.xml file [ID_34269]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When you opened a trend graph, the Y-axis values would incorrectly not take into account the number of decimals configured in the *protocol.xml* file for the parameters in question.

#### DataMiner Cube - Alarm Console: Negative counters in the footer bar [ID_34318]

<!-- Main Release Version 10.2.0 [CU8] - Feature Release Version 10.2.11 -->

On systems with active correlation rules, in some rare cases, the counters in the footer bar of the Alarm Console could show negative numbers.

#### DataMiner Cube - EPM: Not possible to add a second parameter to a trend graph of an EPM object [ID_34323]

<!-- Main Release Version 10.1.0 [CU20]/10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When you opened a trend graph of an EPM object, it would not be possible to add a second parameter. After you had added a new parameter, the drop-down box would incorrectly only contain the current parameter.

#### DataMiner Cube - Visual Overview: Fix multiple script executions on page shape data change [ID_34412]

<!-- Main Release Version 10.2.0 [CU8] - Feature Release Version 10.2.11 -->

When, on page level, you had configured a data field of type *Execute* containing multiple *Set* actions with placeholders as well as a *Script* action, the script would incorrectly get executed multiple times when the page was opened.
