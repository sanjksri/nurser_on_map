<!DOCTYPE html>
<html xmlns="https://www.w3.org/1999/xhtml">
	<head>
		<title>GPS Visualizer map</title>
		<base target="_top"></base>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
		<meta name="viewport" content="initial-scale=1.0, user-scalable=no" />
		
		
	</head>
	<body style="margin:0px;">
		
		<script type="text/javascript">
			API = 'leaflet'; // can be either 'leaflet' or 'google'
			if (self.API && API.match(/^g/i)) {
				google_api_key = ''; // Your project's Google Maps API key goes here (https://code.google.com/apis/console)
				language_code = '';
				document.writeln('<script src="https://maps.googleapis.com/maps/api/js?v=3&amp;libraries=geometry&amp;language='+(self.language_code?self.language_code:'')+'&amp;key='+(self.google_api_key?self.google_api_key:'')+'" type="text/javascript"><'+'/script>');
			} else {
				document.writeln('<link href="https://unpkg.com/leaflet/dist/leaflet.css" rel="stylesheet" />');
				document.writeln('<script src="https://unpkg.com/leaflet/dist/leaflet.js" type="text/javascript"><'+'/script>');
			}
			thunderforest_api_key = ''; // To display OpenStreetMap tiles from ThunderForest, you need a key (https://www.thunderforest.com/docs/apikeys/)
			ign_api_key = ''; // To display topo tiles from IGN.fr, you need a key (https://api.ign.fr/)
		</script>

		
		<!--
			If you want to transplant this map into another Web page, by far the best method is to
			simply include it in a IFRAME tag (see https://www.gpsvisualizer.com/faq.html#google_html).
			But, if you must paste the code into another page, be sure to include all of these parts:
			   1. The "div" tags that contain the map and its widgets, below
			   2. Three sections of JavaScript code:
			      a. The API code (from googleapis.com or unpkg.com/leaflet), above
			      b. "gv_options" and the code that calls a .js file on gpsvisualizer.com
			      c. The "GV_Map" function, which contains all the geographic info for the map
		-->
		<div style="margin-left:0px; margin-right:0px; margin-top:0px; margin-bottom:0px;">
			<div id="gmap_div" style="width:100%; height:100%; margin:0px; margin-right:12px; background-color:#f0f0f0; float:left; overflow:hidden;">
				<p style="text-align:center; font:10px Arial;">This map was created using <a target="_blank" href="https://www.gpsvisualizer.com/">GPS Visualizer</a>'s do-it-yourself geographic utilities.<br /><br />Please wait while the map data loads...</p>
			</div>
				
			<div id="gv_infobox" class="gv_infobox" style="font:13px 'Noto Sans Gujarati'; border:solid #666666 1px; background-color:#ffff99; padding:4px; overflow:auto; display:none; ">
				<p > <b> Map of Gujarat Forest Department Nurseries </b> <br>Anyone can get high quality seedlings at very nominal cost ( Rs 5 - Rs 15 per plant, depending on size) from any of the nurseries shown in this map. For free of cost or concessional rates kindly contact the concerned RFO/DCF. Click on the icon to see more details of the nursery. Call 1926 for more details <br>આ નકશામાં દર્શાવેલ કોઈપણ નર્સરીમાંથી કોઈપણ વ્યક્તિ ખૂબ જ નજીવી કિંમતે (રૂ. 5 - રૂ. 15 પ્રતિ છોડ, થૈલી ના માપ આધારે) ઉચ્ચ ગુણવત્તાવાળા રોપાઓ મેળવી શકે છે. મફત અથવા રાહત દરો માટે, કૃપા કરીને સંબંધિત RFO/DCF  ને સંપર્ક કરવા વિનંતિ છે. નર્સરી ની વધારે માહિતી માટે આયકન પર ક્લિક કરવા વિનંતી છે. વધારે માહિતી માટે 1926 પર ફોન કરવા વિનંતી છે.
</p>
			</div>


			<div id="gv_tracklist" class="gv_tracklist" style="font:11px Arial; line-height:11px; background-color:#ffffff; overflow:auto; display:none;"><!-- --></div>

			<div id="gv_marker_list" class="gv_marker_list" style="background-color:#ffffff; overflow:auto; display:none;"><!-- --></div>

			<div id="gv_clear_margins" style="height:0px; clear:both;"><!-- clear the "float" --></div>
		</div>

		
		<!-- begin GPS Visualizer setup script (must come after loading of API code) -->
		<script type="text/javascript">
			/* Global variables used by the GPS Visualizer functions (20230519044050): */
			gv_options = {};
			
			// basic map parameters:
			gv_options.center = [19,72.3];  // [latitude,longitude] - be sure to keep the square brackets
			gv_options.zoom = 4;  // higher number means closer view; can also be 'auto' for automatic zoom/center based on map elements
			gv_options.map_type = 'GV_HYBRID';  // popular map_type choices are 'GV_STREET', 'GV_SATELLITE', 'GV_HYBRID', 'GV_TERRAIN', 'GV_OSM', 'GV_TOPO_US', 'GV_TOPO_WORLD' (https://www.gpsvisualizer.com/misc/leaflet_map_types.html)
			gv_options.map_opacity = 1.00;  // number from 0 to 1
			gv_options.full_screen = true;  // true|false: should the map fill the entire page (or frame)?
			gv_options.width = 700;  // width of the map, in pixels
			gv_options.height = 700;  // height of the map, in pixels
			
			gv_options.map_div = 'gmap_div';  // the name of the HTML "div" tag containing the map itself; usually 'gmap_div'
			gv_options.doubleclick_zoom = true;  // true|false: zoom in when mouse is double-clicked?
			gv_options.doubleclick_center = true;  // true|false: re-center the map on the point that was double-clicked?
			gv_options.scroll_zoom = true; // true|false; or 'reverse' for down=in and up=out
			gv_options.page_scrolling = true; // true|false; does the map relenquish control of the scroll wheel when embedded in scrollable pages?
			gv_options.autozoom_adjustment = 0; gv_options.autozoom_default = 11;
			gv_options.centering_options = { 'open_info_window':true, 'partial_match':true, 'center_key':'center', 'default_zoom':null } // URL-based centering (e.g., ?center=name_of_marker&zoom=14)
			gv_options.street_view = false; // true|false: allow Google Street View on the map (Google Maps only)
			gv_options.tilt = false; // true|false: allow Google Maps to show 45-degree tilted aerial imagery?
			gv_options.disable_google_pois = false;  // true|false: if you disable clickable POIs on Google Maps, you also lose the labels on parks, airports, etc.
			gv_options.animated_zoom = true; // true|false: only affects Leaflet maps
			
			// widgets on the map:
			gv_options.zoom_control = 'auto'; // 'auto'|'large'|'small'|'none'
			gv_options.recenter_button = true; // true|false: is there a 'click to recenter' button above the zoom control?
			gv_options.geolocation_control = true; // true|false; only works on secure servers
			gv_options.geolocation_options = { center:true, zoom:null, marker:true, info_window:true };
			gv_options.scale_control = true; // true|false
			gv_options.map_opacity_control = false;  // true|false
			gv_options.map_type_control = {};  // widget to change the background map
			  gv_options.map_type_control.visible = 'auto'; // true|false|'auto': is a map type control placed on the map itself?
			  gv_options.map_type_control.filter = false;  // true|false: when map loads, are irrelevant maps ignored?
			  gv_options.map_type_control.excluded = [];  // comma-separated list of quoted map IDs that will never show in the list ('included' also works)
			gv_options.center_coordinates = true;  // true|false: show a "center coordinates" box and crosshair?
			gv_options.measurement_tools = true; // true|false: put a measurement ruler on the map?
			gv_options.measurement_options = { visible:false, distance_color:'', area_color:'' };
			gv_options.crosshair_hidden = true;  // true|false: hide the crosshair initially?
			gv_options.mouse_coordinates = false;  // true|false: show a "mouse coordinates" box?
			gv_options.utilities_menu = { 'maptype':true, 'opacity':true, 'measure':true, 'geolocate':false, 'profile':true, 'export':false };
			gv_options.allow_export = false;  // true|false
			
			gv_options.infobox_options = {}; // options for a floating info box (id="gv_infobox"), which can contain anything
			  gv_options.infobox_options.enabled = true;  // true|false: enable or disable the info box altogether
			  gv_options.infobox_options.position = ['LEFT_TOP',52,4];  // [Google anchor name, relative x, relative y]
			  gv_options.infobox_options.draggable = true;  // true|false: can it be moved around the screen?
			  gv_options.infobox_options.collapsible = true;  // true|false: can it be collapsed by double-clicking its top bar?
			
			// track-related options:
			gv_options.track_optimization = 1; // sets Leaflet's smoothFactor parameter
			gv_options.track_tooltips = false; // true|false: should the name of a track appear on the map when you mouse over the track itself?
			gv_options.tracklist_options = {}; // options for a floating list of the tracks visible on the map
			  gv_options.tracklist_options.enabled = true;  // true|false: enable or disable the tracklist altogether
			  gv_options.tracklist_options.position = ['RIGHT_TOP',4,32];  // [Google anchor name, relative x, relative y]
			  gv_options.tracklist_options.min_width = 100; // minimum width of the tracklist, in pixels
			  gv_options.tracklist_options.max_width = 180; // maximum width of the tracklist, in pixels
			  gv_options.tracklist_options.min_height = 0; // minimum height of the tracklist, in pixels; if the list is longer, scrollbars will appear
			  gv_options.tracklist_options.max_height = 310; // maximum height of the tracklist, in pixels; if the list is longer, scrollbars will appear
			  gv_options.tracklist_options.desc = true;  // true|false: should tracks' descriptions be shown in the list
			  gv_options.tracklist_options.toggle = false;  // true|false: should clicking on a track's name turn it on or off?
			  gv_options.tracklist_options.checkboxes = true;  // true|false: should there be a separate icon/checkbox for toggling visibility?
			  gv_options.tracklist_options.zoom_links = true;  // true|false: should each item include a small icon that will zoom to that track?
			  gv_options.tracklist_options.highlighting = true;  // true|false: should the track be highlighted when you mouse over the name in the list?
			  gv_options.tracklist_options.tooltips = false;  // true|false: should the name of the track appear on the map when you mouse over the name in the list?
			  gv_options.tracklist_options.draggable = true;  // true|false: can it be moved around the screen?
			  gv_options.tracklist_options.collapsible = true;  // true|false: can it be collapsed by double-clicking its top bar?
			  gv_options.tracklist_options.header = 'Tracks:'; // HTML code; be sure to put backslashes in front of any single quotes, and don't include any line breaks
			  gv_options.tracklist_options.footer = ''; // HTML code
			gv_options.profile_options = { visible:false, icon:true, units:'metric', filled:true, waypoints:true, height:120, width:'100%', y_min:null, y_max:null, gap_between_tracks:false }; // see https://www.gpsvisualizer.com/tutorials/profiles_in_maps.html


			// marker-related options:
			gv_options.default_marker = { color:'red',icon:'googlemini',scale:1 }; // icon can be a URL, but be sure to also include size:[w,h] and optionally anchor:[x,y]
			gv_options.vector_markers = true; // are the icons on the map in embedded SVG format?
			gv_options.marker_tooltips = true; // do the names of the markers show up when you mouse-over them?
			gv_options.marker_shadows = true; // true|false: do the standard markers have "shadows" behind them?
			gv_options.marker_link_target = '_blank'; // the name of the window or frame into which markers' URLs will load
			gv_options.info_window_width = 0;  // in pixels, the width of the markers' pop-up info "bubbles" (can be overridden by 'window_width' in individual markers)
			gv_options.thumbnail_width = 0;  // in pixels, the width of the markers' thumbnails (can be overridden by 'thumbnail_width' in individual markers)
			gv_options.photo_size = [0,0];  // in pixels, the size of the photos in info windows (can be overridden by 'photo_width' or 'photo_size' in individual markers)
			gv_options.hide_labels = false;  // true|false: hide labels when map first loads?
			gv_options.labels_behind_markers = false; // true|false: are the labels behind other markers (true) or in front of them (false)?
			gv_options.label_offset = [0,0];  // [x,y]: shift all markers' labels (positive numbers are right and down)
			gv_options.label_centered = false;  // true|false: center labels with respect to their markers?  (label_left is also a valid option.)
			gv_options.driving_directions = false;  // put a small "driving directions" form in each marker's pop-up window? (override with dd:true or dd:false in a marker's options)
			gv_options.garmin_icon_set = 'gpsmap'; // 'gpsmap' are the small 16x16 icons; change it to '24x24' for larger icons
			gv_options.marker_list_options = {};  // options for a dynamically-created list of markers
			  gv_options.marker_list_options.enabled = false;  // true|false: enable or disable the marker list altogether
			  gv_options.marker_list_options.floating = true;  // is the list a floating box inside the map itself?
			  gv_options.marker_list_options.position = ['RIGHT_BOTTOM',6,38];  // floating list only: position within map
			  gv_options.marker_list_options.min_width = 160; // minimum width, in pixels, of the floating list
			  gv_options.marker_list_options.max_width = 160;  // maximum width
			  gv_options.marker_list_options.min_height = 0;  // minimum height, in pixels, of the floating list
			  gv_options.marker_list_options.max_height = 310;  // maximum height
			  gv_options.marker_list_options.draggable = true;  // true|false, floating list only: can it be moved around the screen?
			  gv_options.marker_list_options.collapsible = true;  // true|false, floating list only: can it be collapsed by double-clicking its top bar?
			  gv_options.marker_list_options.include_tickmarks = false;  // true|false: are distance/time tickmarks included in the list?
			  gv_options.marker_list_options.include_trackpoints = false;  // true|false: are "trackpoint" markers included in the list?
			  gv_options.marker_list_options.dividers = false;  // true|false: will a thin line be drawn between each item in the list?
			  gv_options.marker_list_options.desc = false;  // true|false: will the markers' descriptions be shown below their names in the list?
			  gv_options.marker_list_options.icons = true;  // true|false: should the markers' icons appear to the left of their names in the list?
			  gv_options.marker_list_options.thumbnails = false;  // true|false: should markers' thumbnails be shown in the list?
			  gv_options.marker_list_options.folders_collapsed = false;  // true|false: do folders in the list start out in a collapsed state?
			  gv_options.marker_list_options.folders_hidden = false;  // true|false: do folders in the list start out in a hidden state?
			  gv_options.marker_list_options.collapsed_folders = []; // an array of folder names
			  gv_options.marker_list_options.hidden_folders = []; // an array of folder names
			  gv_options.marker_list_options.count_folder_items = false;  // true|false: list the number of items in each folder?
			  gv_options.marker_list_options.folder_zoom = true;  // true|false: is there a zoom link next to each folder name?
			  gv_options.marker_list_options.wrap_names = true;  // true|false: should marker's names be allowed to wrap onto more than one line?
			  gv_options.marker_list_options.unnamed = '[unnamed]';  // what 'name' should be assigned to  unnamed markers in the list?
			  gv_options.marker_list_options.colors = false;  // true|false: should the names/descs of the points in the list be colorized the same as their markers?
			  gv_options.marker_list_options.default_color = '';  // default HTML color code for the names/descs in the list
			  gv_options.marker_list_options.limit = 0;  // how many markers to show in the list; 0 for no limit
			  gv_options.marker_list_options.center = false;  // true|false: does the map center upon a marker when you click its name in the list?
			  gv_options.marker_list_options.zoom = false;  // true|false: does the map zoom to a certain level when you click on a marker's name in the list?
			  gv_options.marker_list_options.zoom_level = 11;  // if 'zoom' is true, what level should the map zoom to?
			  gv_options.marker_list_options.info_window = true;  // true|false: do info windows pop up when the markers' names are clicked in the list?
			  gv_options.marker_list_options.url_links = false;  // true|false: do the names in the list become instant links to the markers' URLs?
			  gv_options.marker_list_options.toggle = false;  // true|false: does a marker disappear if you click on its name in the list?
			  gv_options.marker_list_options.help_tooltips = false;  // true|false: do "tooltips" appear on marker names that tell you what happens when you click?
			  gv_options.marker_list_options.id = 'gv_marker_list';  // id of a DIV tag that holds the list
			  gv_options.marker_list_options.header = ''; // HTML code; be sure to put backslashes in front of any single quotes, and don't include any line breaks
			  gv_options.marker_list_options.footer = ''; // HTML code
			gv_options.marker_filter_options = {};  // options for removing waypoints that are out of the current view
			  gv_options.marker_filter_options.enabled = false;  // true|false: should out-of-range markers be removed?
			  gv_options.marker_filter_options.movement_threshold = 8;  // in pixels, how far the map has to move to trigger filtering
			  gv_options.marker_filter_options.limit = 0;  // maximum number of markers to display on the map; 0 for no limit
			  gv_options.marker_filter_options.update_list = true;  // true|false: should the marker list be updated with only the filtered markers?
			  gv_options.marker_filter_options.sort_list_by_distance = false;  // true|false: should the marker list be sorted by distance from the center of the map?
			  gv_options.marker_filter_options.min_zoom = 0;  // below this zoom level, don't show any markers at all
			  gv_options.marker_filter_options.zoom_message = '';  // message to put in the marker list if the map is below the min_zoom threshold
			gv_options.synthesize_fields = {}; // for example: {label:'{name}'} would cause all markers' names to become visible labels
				

			
			// Load GPS Visualizer's mapping functions (this must be loaded AFTER gv_options are set):
			var script_file = (self.API && API.match(/^g/i)) ? 'google_maps/functions3.js' : 'leaflet/functions.js';
			if (document.location.protocol == 'https:') { // secure pages require secure scripts
				document.writeln('<script src="https://www.gpsvisualizer.com/'+script_file+'" type="text/javascript"><'+'/script>');
			} else {
				document.writeln('<script src="http://maps.gpsvisualizer.com/'+script_file+'" type="text/javascript"><'+'/script>');
			}
		</script>
		<style type="text/css">
			/* Put any custom style definitions here (e.g., .gv_marker_info_window, .gv_marker_info_window_name, .gv_marker_list_item, .gv_tooltip, .gv_label, etc.) */
			#gmap_div .gv_marker_info_window {
				font-size:11px !important;
			}
			#gmap_div .gv_label {
				opacity:0.90; filter:alpha(opacity=90);
				color:white; background:#333333; border:1px solid black; padding:1px;
				font-family:Verdana !important; font-size:10px;
				font-weight:normal !important;
			}
			.legend_block {
				display:inline-block; border:solid 1px black; width:9px; height:9px; margin:0px 2px 0px 0px;
			}
			
		</style>
		
		<!-- end GPSV setup script and styles; begin map-drawing script (they must be separate) -->
		<script type="text/javascript">
			function GV_Map() {
				GV_Setup_Map();
				
				
				
				// This set of options instructs the "GV_Finish_Map" function to load markers from an external file
				gv_options.dynamic_data = [
					{
					url:'https://docs.google.com/spreadsheets/d/1p7DPvp87KjSb1KCNqJTiormVrHMGxrepcy3TDwCgs_Y/edit#gid=1354678438', reload_on_move:false,
					field_alias:{}, // e.g.: field_alias:{name:'id',desc:'comment',folder:'category'}
					synthesize_fields:{ // you can include YOUR document's field names in {curly brackets}; this is like field_alias, but more powerful
						name:'',
						desc:'',
						label:'',
						folder:''
					},
					ignore_styles:false,
					track_options:{color:'#e60000',width:'3',opacity:'0.9'},
					autozoom:true, zoom_default:8, zoom_adjustment:0 // e.g., to zoom out one step, set zoom_adjustment to -1
					}
				];
				
				GV_Finish_Map();
					
			}
			GV_Map(); // execute the above code
			// https://www.gpsvisualizer.com/map_input?form:dynamic_data=https%3A%2F%2Fdocs.google.com%2Fspreadsheets%2Fd%2F1p7DPvp87KjSb1KCNqJTiormVrHMGxrepcy3TDwCgs_Y%2Fedit%23gid%3D1354678438&form=leaflet&geolocation_control=1&legend_html=%3Cp%20style%3D%22background-color%3Ayellow%3B%22%3EAnyone%20can%20get%20high%20quality%20seedlings%20with%20very%20nominal%20cost%20%28%20Rs%205%20-%20Rs%2020%20per%20plant%2C%20depending%20on%20size%29%20from%20any%20of%20the%20nurseries%20shown%20in%20this%20map.%20For%20free%20of%20cost%20or%20concessional%20rates%20kindly%20contact%20the%20concerned%20DCF.%20Click%20on%20the%20icon%20to%20see%20more%20details%20of%20the%20nursery.%20%3Cbr%3E%0D%0A%E0%AA%86%20%E0%AA%A8%E0%AA%95%E0%AA%B6%E0%AA%BE%E0%AA%AE%E0%AA%BE%E0%AA%82%20%E0%AA%A6%E0%AA%B0%E0%AB%8D%E0%AA%B6%E0%AA%BE%E0%AA%B5%E0%AB%87%E0%AA%B2%20%E0%AA%95%E0%AB%8B%E0%AA%88%E0%AA%AA%E0%AA%A3%20%E0%AA%A8%E0%AA%B0%E0%AB%8D%E0%AA%B8%E0%AA%B0%E0%AB%80%E0%AA%AE%E0%AA%BE%E0%AA%82%E0%AA%A5%E0%AB%80%20%E0%AA%95%E0%AB%8B%E0%AA%88%E0%AA%AA%E0%AA%A3%20%E0%AA%B5%E0%AB%8D%E0%AA%AF%E0%AA%95%E0%AB%8D%E0%AA%A4%E0%AA%BF%20%E0%AA%96%E0%AB%82%E0%AA%AC%20%E0%AA%9C%20%E0%AA%A8%E0%AA%9C%E0%AB%80%E0%AA%B5%E0%AB%80%20%E0%AA%95%E0%AA%BF%E0%AA%82%E0%AA%AE%E0%AA%A4%E0%AB%87%20%28%E0%AA%B0%E0%AB%82.%205%20-%20%E0%AA%B0%E0%AB%82.%2020%20%E0%AA%AA%E0%AB%8D%E0%AA%B0%E0%AA%A4%E0%AA%BF%20%E0%AA%9B%E0%AB%8B%E0%AA%A1%20%29%20%E0%AA%89%E0%AA%9A%E0%AB%8D%E0%AA%9A%20%E0%AA%97%E0%AB%81%E0%AA%A3%E0%AA%B5%E0%AA%A4%E0%AB%8D%E0%AA%A4%E0%AA%BE%E0%AA%B5%E0%AA%BE%E0%AA%B3%E0%AA%BE%20%E0%AA%B0%E0%AB%8B%E0%AA%AA%E0%AA%BE%E0%AA%93%20%E0%AA%AE%E0%AB%87%E0%AA%B3%E0%AA%B5%E0%AB%80%20%E0%AA%B6%E0%AA%95%E0%AB%87%20%E0%AA%9B%E0%AB%87.%20%E0%AA%AE%E0%AA%AB%E0%AA%A4%20%E0%AA%85%E0%AA%A5%E0%AA%B5%E0%AA%BE%20%E0%AA%B0%E0%AA%BE%E0%AA%B9%E0%AA%A4%20%E0%AA%A6%E0%AA%B0%E0%AB%8B%20%E0%AA%AE%E0%AA%BE%E0%AA%9F%E0%AB%87%2C%20%E0%AA%95%E0%AB%83%E0%AA%AA%E0%AA%BE%20%E0%AA%95%E0%AA%B0%E0%AB%80%E0%AA%A8%E0%AB%87%20%E0%AA%B8%E0%AA%82%E0%AA%AC%E0%AA%82%E0%AA%A7%E0%AA%BF%E0%AA%A4%20%E0%AA%A1%E0%AB%80%E0%AA%B8%E0%AB%80%E0%AA%8F%E0%AA%AB%E0%AA%A8%E0%AB%8B%20%E0%AA%B8%E0%AA%82%E0%AA%AA%E0%AA%B0%E0%AB%8D%E0%AA%95%20%E0%AA%95%E0%AA%B0%E0%AB%8B.%20%E0%AA%A8%E0%AA%B0%E0%AB%8D%E0%AA%B8%E0%AA%B0%E0%AB%80%E0%AA%A8%E0%AB%80%20%E0%AA%B5%E0%AA%A7%E0%AB%81%20%E0%AA%B5%E0%AA%BF%E0%AA%97%E0%AA%A4%E0%AB%8B%20%E0%AA%9C%E0%AB%8B%E0%AA%B5%E0%AA%BE%20%E0%AA%AE%E0%AA%BE%E0%AA%9F%E0%AB%87%20%E0%AA%86%E0%AA%AF%E0%AA%95%E0%AA%A8%20%E0%AA%AA%E0%AA%B0%20%E0%AA%95%E0%AB%8D%E0%AA%B2%E0%AA%BF%E0%AA%95%20%E0%AA%95%E0%AA%B0%E0%AB%8B.%3C%2Fp%3E&units=metric
		</script>
		
		
		
	</body>

</html>
