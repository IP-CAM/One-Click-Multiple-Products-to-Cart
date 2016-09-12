/*
 * @support
 * http://www.opensourcetechnologies.com/contactus.html
 * sales@opensourcetechnologies.com
 * */
$(document).ready(function() {
//One Click Multiple Products To Cart Starting
	
	$('.selectall').click(function()
	{
		if( $(this).prop('checked') )
		{
			$('.selectall').prop('checked','checked');
			$('.checks').prop('checked','checked');
		}
		else
		{
			$('.checks').removeAttr('checked','checked');
			$('.selectall').removeAttr('checked','checked');
		}
	}
	);
	$('.plusqty').click(function()
		{
			var qty=$('.qty').eq(0).val();
			qty=Number(qty)+1;
			$('.qty').val(qty);
			$('.quantity').val(qty);
		}	
	);
	$('.minusqty').click(function()
		{
			var qty=Number($('.qty').eq(0).val());
			if(qty!=0)
			qty=qty-1;
			$('.qty').val(qty);
			$('.quantity').val(qty);
		}	
	);
	$('.qty').change(function()
		{
			var qty=Number($(this).val());
			$('.qty').val(qty);
			$('.quantity').val(qty);
		}
	);
	$('.bulk-buy-button').click(function()
		{
			
			$('.checks').each(function(index)
				{
					
					if( $(this).prop('checked') )
					{
						var val=$('.quantity').eq(index).val();
						var id_string=	$('.quantity').eq(index).attr('id');
						var ids=id_string.split('_');
						if(val!=0)
						cart.add(ids[1],val);
					}
				}
			);
		}
	);
	//$('.')
	//Bulk Buy Ending
});	
