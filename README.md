# Level Up Your Life With Custom Meta

An introduction to the **Advanced Custom Fields** plugin for the MSP Wordpress Meetup Group.

## Example #1

### How to use ACF *shortcodes* on your site to show your custom meta field values
Make an "event" post for a fictional company by adding custom meta values for the "event" to a sidebar widget that appears only on Wordpress Posts that have the category *Event*.

### Plugins Used

#### Advanced Custom Fields
https://wordpress.org/plugins/advanced-custom-fields/

#### Shortcode Widget plugin
https://wordpress.org/plugins/shortcode-widget/

#### Display Widgets plugin
https://wordpress.org/plugins/display-widgets/

### Field Group Used

[advanced-custom-field-export.xml](https://github.com/mcurren/acf-meetup-examples/blob/master/advanced-custom-field-export.xml "Event Details ACF Field Group")

### Shortcodes Used in Widget

    <strong>Date</strong>  
    [acf field=event_date]

    <strong>Time</strong>  
    [acf field=event_time]

    <strong>Venue</strong>  
    [acf field=event_address]

## Example #2

### How to use ACF *template tags* on your site to show your custom meta field values
Make an "event" landing page for the same fictional company by adding custom meta values for the "event" to a custom page template in your child theme.

### Plugins Used

#### Advanced Custom Fields
https://wordpress.org/plugins/advanced-custom-fields/

### Field Group Used

[advanced-custom-field-export.xml](https://github.com/mcurren/acf-meetup-examples/blob/master/advanced-custom-field-export.xml "Event Details ACF Field Group")

### Template Tags & HTML Used in Page Template

    <div class="event-details">

        <h3>Event Details</h3>

        <p>
            <strong>Date</strong><br>
            <?php the_field('event_date'); ?>
        </p>

        <p>
            <strong>Time</strong><br>
            <?php the_field('event_time'); ?>
        </p>

        <p>
            <strong>Location</strong><br>
            <?php the_field('event_address'); ?>
        </p>

    </div><!-- .event-details -->

