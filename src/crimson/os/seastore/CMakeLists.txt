add_library(crimson-seastore STATIC
  cached_extent.cc
  seastore_types.cc
  segment_manager/ephemeral.cc
  segment_manager.cc
  transaction_manager.cc
  journal.cc
  cache.cc
  lba_manager.cc
  lba_manager/btree/btree_lba_manager.cc
  lba_manager/btree/lba_btree_node_impl.cc
  lba_manager/btree/btree_range_pin.cc
  onode.cc
  onode_manager/simple-fltree/onode_block.cc
  onode_manager/simple-fltree/onode_delta.cc
  onode_manager/simple-fltree/onode_node.cc
  seastore.cc
  ../../../test/crimson/seastore/test_block.cc
	)
target_link_libraries(crimson-seastore
  crimson
  crimson-os)

