# Panel Utils 
This repository contains a frequently used methods in BentoBox addons that I create.

### Main PanelUtils class contains methods:

```
/**
 * This method sets blocks with given Material around Panel with given row count.
 * @param panelBuilder object that builds Panel.
 * @param rowCount in Panel.
 * @param material that will be around Panel.
 */
PanelUtils#fillBorder(PanelBuilder panelBuilder, int rowCount, Material material)

/**
 * This method transforms entity into player head with skin that corresponds given
 * entity. If entity head is not found, then it is replaced by barrier block.
 * @param entity which head must be returned.
 * @param amount of ItemStack elements.
 * @return ItemStack that may be head for given entity.
 */
PanelUtils#getEntityHead(EntityType entity, int amount)

/**
 * This method transforms entity into egg or block that corresponds given entity.
 * If entity egg is not found, then it is replaced by block that represents entity or
 * barrier block.
 * @param entity which egg must be returned.
 * @param amount of ItemStack elements.
 * @return ItemStack that may be egg for given entity.
 */
PanelUtils#getEntityEgg(EntityType entity, int amount)

/**
 * This method transforms material into item stack that can be displayed in users
 * inventory, as not all materials can be displayed.
 * @param material which item stack must be returned.
 * @param amount of ItemStack elements.
 * @return ItemStack that represents given material.
 */
PanelUtils#getMaterialItem(Material material, int amount)
```

### Main MobHeadContainer method:

```
/**
 * Returns an ItemStack of the custom head.
 *
 * @param amount of items in the stack
 * @param displayName the name to display. Supports "&amp;" color codes
 * @param loreLines   optional lore lines. Supports "&amp;" color codes
 * @return an ItemStack of the custom head.
 */
MobHeadContainer#toItemStack(int amount, String displayName, String... loreLines)
```