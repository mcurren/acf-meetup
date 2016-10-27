# Example #1

## How to use ACF *shortcodes* on your site to show your custom meta field values.
Make an "event" post for a fictional company by adding custom meta values for the "event" to a sidebar widget that appears only on Wordpress Posts that have the category *Event*.

## Plugins Used

### Advanced Custom Fields
https://wordpress.org/plugins/advanced-custom-fields/

### Shortcode Widget plugin
https://wordpress.org/plugins/shortcode-widget/

### Display Widgets plugin
https://wordpress.org/plugins/display-widgets/

## Field Group Used

(link)

## Shortcodes Used in Widget

    <strong>Date</strong>  
    [acf field=event_date]

    <strong>Time</strong>  
    [acf field=event_time]

    <strong>Venue</strong>  
    [acf field=event_address]

# Example #2

## How to use ACF *template tags* on your site to show your custom meta field values.
Make an "event" landing page for the same fictional company by adding custom meta values for the "event" to a custom page template in your child theme.

## Plugins Used

### Advanced Custom Fields
https://wordpress.org/plugins/advanced-custom-fields/

## Template Tags Used in Widget

    <div class="event-details">

        <h3>Event Details</h3>

        <h4>Date</h4>
        <p><?php the_field('event_date'); ?></p>

        <h4>Time</h4>
        <p><?php the_field('event_time'); ?></p>

        <h4>Location</h4>
        <p><?php the_field('event_address'); ?></p>

    </div><!-- .event-details -->

